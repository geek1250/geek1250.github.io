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

<p>use adb -s "emulatorName" before command to select a device 

<p>example: install an app
<p>
adb -s emulator-5554 install test.apk

