---
layout: post
title:  "how to fix the issue that CSS file does not show the latest content"
subtitle: ""
categories: ""
author: Geek
date:   2019-07-06 15:34:56 -0400
background: '/img/posts/01.jpg'
---
Observation:
A css file uses version when it is called like style.css?ver=5.2.1.
However, Chrome broswer could not get the latest content even after force flush and disable cache on the developer tools.
<br>
Root reason:Server time is behind the current time. The latest change could not take effect.
<br>
How to fix:

Change server time to the current time. And then force flush the page. It does not which time zone the server is using. Just make sure that the corrosponding time is consistent to the current time.
