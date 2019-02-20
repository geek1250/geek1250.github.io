---
layout: post
title:  "osstatus"
subtitle: ""
categories: ""
author: Geek
date:   2019-02-20 16:54:56 -0400
background: '/img/posts/02.jpg'
---
If you're getting something like this when run iOS app in XCode:

App has conflicting provisioning settings. App is automatically signed, but provisioning profile 'ID' has been manually specified. Set the provisioning profile value to "Automatic" in the build settings editor, or switch to manual signing in the project editor.
<br>
Fix method:
<br>
empty PROVISIONING_PROFILE option in Build Setting in Xcode
