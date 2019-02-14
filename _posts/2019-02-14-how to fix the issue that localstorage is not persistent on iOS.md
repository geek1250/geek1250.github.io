---
layout: post
title:  "how to fix the issue that localstorage is not persistent on iOS"
subtitle: ""
categories: ""
author: Geek
date:   2019-02-14 15:54:56 -0400
background: '/img/posts/01.jpg'
---

At the beginning, I thought it is an issue related to Cordova (https://issues.apache.org/jira/browse/CB-12509)
<br>
However, we fixed it by changing 
<br><preference name="BackupWebStorage" value="local" /> to    
<br><preference name="BackupWebStorage" value="cloud" />
<br>
in platforms/ios/config.xml
<br>
