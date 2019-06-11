---
layout: post
title:  "how to show content of .mobileprovision file and .cert file"
subtitle: ""
categories: ""
author: Geek
date:   2019-06-11 15:54:56 -0400
background: '/img/posts/05.jpg'
---
show content of .mobileprovision file:
<br>
security cms -D -i iphone-distribution-exsmple.mobileprovision

<p>
show content of .cert file:
<br>openssl x509 -inform der -in Certificates-example.cer -noout -text
