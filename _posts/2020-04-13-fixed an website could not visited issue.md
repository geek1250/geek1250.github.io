---
layout: post
title:  "fixed an issue that a website could not be visited "
subtitle: ""
categories: ""
author: Geek
date:   2020-04-13 19:26:56 -0400
background: '/img/posts/02.jpg'
---
a website based on Flask became unreachable after one day. However, other websites on the same server worked fine.

root reason:
worker_connections is bigger that the ability of CPU in Nginx's default configuratin file nginx.conf

How to fix:
If the server is one core CPU, the max value of worker_connections should be 1024.
If it has b CPUS, the the max value of worker_connections should be 1024*n.

worker_rlimit_nofile is also needed to change. Value is same as worker_connections.
