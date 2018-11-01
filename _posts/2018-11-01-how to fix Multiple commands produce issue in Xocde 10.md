---
layout: post
title:  "how to fix Multiple commands produce issue in Xocde 10"
subtitle: ""
categories: ""
author: Geek
date:   2018-11-01 15:34:56 -0400
background: '/img/posts/04.jpg'
---
way 1: 
<p>
In Xcode, go to File->Project/Workspace settings.
<br>
Change the build system to Legacy Build system.
<br>
https://stackoverflow.com/questions/50718018/xcode-10-error-multiple-commands-produce

<br>
way 2: 
<p>remove one file with same name in "Copy Bundle Resourrces" in Build Phases in Xcode
<br>
I met same this error: two Localizable.strings files are copied from separate location. It is fixed by removing one Localizable.strings file.

<br>
way 3: 
<p>Check "Copy only when installing"
<br>
https://github.com/wix/react-native-navigation/issues/3608
