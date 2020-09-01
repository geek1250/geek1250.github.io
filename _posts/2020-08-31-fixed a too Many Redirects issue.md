---
layout: post
title:  "fixed a too Many Redirects issue"
subtitle: ""
categories: ""
author: Geek
date:   2020-08-31 19:26:56 -0400
background: '/img/posts/03.jpg'
---
Nginx configuration is right but it still gets too Many Redirects issue.
The domain is DNS and SSL set in Cloudflare.com


How to fix:
If you’re receiving the ERR_TOO_MANY_REDIRECTS error when accessing your HTTPS enabled site that is being proxied through Cloudflare, it’s likely that you have SSL set to Flexible. This should be set to Full (strict), which will ensure connections to your site are fully encrypted end-to-end.

The SSL setting can be found under the SSL/TLS tab.
