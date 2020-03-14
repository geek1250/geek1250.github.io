---
layout: post
title:  "fix No module named 'google_auth_oauthlib'"
subtitle: ""
categories: ""
author: Geek
date:   2020-03-14 15:54:56 -0400
background: '/img/posts/01.jpg'
---
fixed by the following suggestion:
make sure you installed the package for the correct python version

bg:
https://developers.google.com/youtube/v3/quickstart/python

Although Google says "Python 2.7 or Python 3.5+" and my machine is python 2.7. But it does not work for me.
Installing the library in python 3.6.9 works for me!
