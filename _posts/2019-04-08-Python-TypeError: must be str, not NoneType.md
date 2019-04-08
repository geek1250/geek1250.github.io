---
layout: post
title:  "Python 3.6: TypeError: must be str, not NoneType"
subtitle: ""
categories: ""
author: Geek
date:   2019-04-08 15:54:56 -0400
background: '/img/posts/04.jpg'
---
Python Error:
<br>
TypeError: must be str, not NoneType

<p>
How to Fix:
<br>
add DocStrings in the very begin of the method
<br>
example:
<br>
def this_is_the_method(self):
<br>    
    """This is the DocStrings"""
    
    
<br>
What is a Docstring?
<br>
https://www.python.org/dev/peps/pep-0257/
<br>
A docstring is a string literal that occurs as the first statement in a module, function, class, or method definition. Such a docstring becomes the __doc__ special attribute of that object.
<br>
All modules should normally have docstrings, and all functions and classes exported by a module should also have docstrings. Public methods (including the __init__ constructor) should also have docstrings. A package may be documented in the module docstring of the __init__.py file in the package directory.


