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
However, we fixed it by changing the value of BackupWebStorage preference from local to cloud in platforms/ios/config.xml
<br>
<code class="ruby">
<preference name="BackupWebStorage" value="local" />
</code> to    
<br>
<code class="ruby">
  <preference name="BackupWebStorage" value="cloud" />
</code>
<br>
BackupWebStorage (string, either none, local, or the default cloud): Set to cloud to allow web storage data to backup via iCloud. Set to local to allow only local backups via iTunes sync. Set to none prevent web storage backups.
<br>https://cordova.apache.org/docs/en/5.1.1/guide/platforms/ios/config.html

