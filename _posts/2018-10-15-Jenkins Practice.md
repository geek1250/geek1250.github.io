---
layout: post
title:  "Jenkins Practice"
subtitle: ""
categories: ""
author: Geek
date:   2018-10-15 15:34:56 -0400
background: '/img/posts/06.jpg'
---

Download and run Jenkins
<p>
Download Jenkins from http://mirrors.jenkins.io/war-stable/latest/jenkins.war

Open up a terminal in the download directory.

Run java -jar jenkins.war --httpPort=8080.

Browse to http://localhost:8080.

Follow the instructions to complete the installation.

<p> or run it by script
1) vim jenkins.sh
2)input the following content in it 
#!/bin/sh
# Run Jenkins
java -jar jenkins.war --httpPort=8080
  
3)chmod a+rx jenkins.sh
4) ./jenkins.sh

Plugins:
add Git Parameter if you build need parameter

  


