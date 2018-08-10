---
layout: post
title:  "how to select Android device"
subtitle: ""
categories: ""
author: Ha
date:   2018-08-09 11:34:56 -0400
background: '/img/posts/06.jpg'
---

<p>
use "adb devices" to show all devices includeing emulators
  
<p> result example:
<br>List of devices attached
<br>1b003d2b	device
<br>emulator-5554	device

<p>use adb -s "Device ID" before command to select a device 

<p>example: install an app
<p>
adb -s emulator-5554 install test.apk

