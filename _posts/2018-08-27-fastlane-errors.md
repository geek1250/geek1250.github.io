---
layout: post
title:  "fastlane errors"
subtitle: ""
categories: ""
author: Ha
date:   2018-08-27 15:34:56 -0400
background: '/img/posts/02.jpg'
---
Error 1
<p>
Failed: Incorrect, or missing copyright date-> using a copyright date that is any different from this current year, or missing a date ... copyright | missing: 2018
<p>
Reason:
<p>
 the Copyright information in Apple iTunes does not contain the current year.


<p>
 when delivering an app, precheck function in fastlane can "check your app using a community driven set of App Store review rules to avoid being rejected" (https://docs.fastlane.tools/actions/precheck/).
<p>

<p>
Error 2
<p>
"Could not find a version to edit for app 'here is the app name', the app metadata is read-only currently".
<p>
Reason
<p>
skip_app_version_update  is set to true which causes we cannot create a new version in iTunes with the same ipa build version number. 
