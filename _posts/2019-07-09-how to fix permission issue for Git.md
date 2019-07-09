---
layout: post
title:  "how to fix permission issue for Git"
subtitle: ""
categories: ""
author: Geek
date:   2019-07-09 15:34:56 -0400
background: '/img/posts/02.jpg'
---
First, check according to to the Github's document.
If it still does not work, it might can be fixed by adding private key in command line as follow:
ssh-git YOURPRIVATEKEY
YOURPRIVATEKEY is locted in /Users/YOURUSERNAME/.ssh folder.

However, if you close the your PC, it will invalid. You need to add it again or add it in your /Users/YOURUSERNAME/.bash_profile file.
