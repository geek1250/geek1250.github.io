---
layout: post
title:  "fixed an error for Agora for Flutter"
subtitle: ""
categories: ""
author: Geek
date:   2019-10-04 15:34:56 -0400
background: '/img/posts/04.jpg'
---
The demo https://github.com/AgoraIO-Community/Agora-Flutter-Quickstart has an issue:
Unable to find a specification for `AgoraRtcEngine_iOS_Crypto (= 2.4.1)` depended upon by `agora_rtc_engine`

Agora version: 0.9.7
Flutter version:1.5.4-hotfix.2

How was it fixed:
run "pod repo update" in the flutter folder



But on the latest Agora Version 1.0.0, its official demo has error "Too many positional arguments: 1 expected, but 2 found":
AgoraRtcEngine.createNativeView { 	"resource": "Agora-Flutter-Quickstart-master/lib/src/pages/call.dart", 	"owner": "dart", 	"code": "extra_positional_arguments_could_be_named", 	"severity": 8, 	"message": "Too many positional arguments: 1 expected, but 2 found.\nTry removing the extra positional arguments, or specifying the name for named arguments
