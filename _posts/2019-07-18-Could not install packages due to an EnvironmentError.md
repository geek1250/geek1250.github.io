---
layout: post
title:  "Could not install packages due to an EnvironmentError"
subtitle: ""
categories: ""
author: Geek
date:   2019-07-1 815:34:56 -0400
background: '/img/posts/02.jpg'
---

When run "sudo pip install pipenv" in command line on Mac (MacOS Mojave Version:10.14.5), it gives an error as below:

Could not install packages due to an EnvironmentError: [('/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/_markerlib/markers.pyc', '/private/tmp/pip-uninstall-xCXo0p/markers.pyc', "[Errno 1] Operation not permitted: '/private/tmp/pip-uninstall-xCXo0p/markers.pyc'"), ('/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/_markerlib/__init__.py', '/private/tmp/pip-uninstall-xCXo0p/__init__.py', "[Errno 1] Operation not permitted: '/private/tmp/pip-uninstall-xCXo0p/__init__.py'"), ('/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/_markerlib/markers.py', '/private/tmp/pip-uninstall-xCXo0p/markers.py', "[Errno 1] Operation not permitted: '/private/tmp/pip-uninstall-xCXo0p/markers.py'"), ('/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/_markerlib/__init__.pyc', '/private/tmp/pip-uninstall-xCXo0p/__init__.pyc', "[Errno 1] Operation not permitted: '/private/tmp/pip-uninstall-xCXo0p/__init__.pyc'"), ('/System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python/_markerlib', '/private/tmp/pip-uninstall-xCXo0p', "[Errno 1] Operation not permitted: '/private/tmp/pip-uninstall-xCXo0p'")]

How to fix it:
sudo python -m pip install pipenv

-m mod : run library module as a script (terminates option list)
