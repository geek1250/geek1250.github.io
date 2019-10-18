--
layout: post
title:  "fix flutter_facebook_login plugin"
subtitle: ""
categories: ""
author: Geek
date:   2019-10-17 15:34:56 -0400
background: '/img/posts/05.jpg'
---

flutter_facebook_login: version 3.0.0
issue:
    [!] Automatically assigning platform `iOS` with version `8.0` on target `Runner` because no platform was specified. Please specify a platform for this target in your Podfile. See `https://guides.cocoapods.org/syntax/podfile.html#platform`.


Error running pod install

How to fix:
method 1:
add platform :ios, '9.0' in file ios/Podfile

method 1:
change s.ios.deployment_target = '9.0' to s.ios.deployment_target = '8.0'in file: ios/.symlinks/plugins/flutter_facebook_login/ios/flutter_facebook_login.podspec
s.ios.deployment_target = '9.0'
