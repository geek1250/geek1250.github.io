---
layout: post
title:  "Fix the issue that dlib install failure"
subtitle: ""
categories: ""
author: Geek
date:   2021-03-04 10:26:56 -0400
background: '/img/posts/06.jpg'
---
pip install dlib
fails at :
Building wheels for collected packages: dlib
  Building wheel for dlib (setup.py) .
  
  
Fix:  
pip install dlib -vvv
