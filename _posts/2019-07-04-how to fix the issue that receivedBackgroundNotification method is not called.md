---
layout: post
title:  "how to fix the issue that receivedBackgroundNotification method is not called"
subtitle: ""
categories: ""
author: Geek
date:   2019-07-04 15:34:56 -0400
background: '/img/posts/06.jpg'
---
If "content-available": true is added in the Payload of the Test Push in UrbanShip console UI, the method 
<br>
(void)receivedBackgroundNotification:(NSDictionary *)notification fetchCompletionHandler:(void (^)(UIBackgroundFetchResult result))completionHandler will be called.

<br>
Sourece:
<br>
“If you fail to include this flag(content-available flag) in the notification, your app will not receive any protocol method calls when the notification arrives” in https://medium.com/posts-from-emmerge/ios-push-notification-background-fetch-demystified-7090358bb66e
