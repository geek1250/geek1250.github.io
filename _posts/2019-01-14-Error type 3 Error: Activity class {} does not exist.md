---
layout: post
title:  "Android - Error type 3 Error: Activity class {} does not exist"
subtitle: ""
categories: ""
author: Geek
date:   2019-01-14 15:34:56 -0400
background: '/img/posts/05.jpg'
---

This is because the Android app that you are trying to load is still installed for another user account on the same device. 
Some devices like Samsung, Huawei can have multipal Users and each user has its own UI and space. 
Some apps are installed for the different users even the app looks only installed for the current user.
To verify this senario, you can switch the accout/user on Setting and you should see the app is installed for the user you switch to. Actually, it is installed for all users.

<br>
Once the app is uninstalled on the current user, there are two ways to fix the issue.
1. switch to each account/user and uninstall the app
2. use Android Studio to generate an APK file, install it and uninstall for all users.
   steps:
    1)Go to Settings.
    2)Go to Apps.
    3)Select your app.
    4)Open the overflow menu on the top right and select Uninstall for all users.
   
 to avoid the issue, it is recommended to uninstall an app for all users by switching to apps in settings. 
 Draging an app to uninstall on desktop is not the right way to uninstall it.


