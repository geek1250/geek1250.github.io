---
layout: post
title:  "how to fix iframe does not work issue on Cordova project for iOS"
subtitle: ""
categories: ""
author: Geek
date:   2019-02-06 16:34:56 -0400
background: '/img/posts/01.jpg'
---
Issue: iframe could not load and shows blank on Cordova 8.
<br>
Background: upgrade Cordova project from Cordova 5 to Cordova 8.
<br>
Reason: Feature IntentAndNavigationFilter is not added to the new Cordova 8 project. The feature IntentAndNavigationFilter is created and used by default when creating a new Cordova app on Cordova 8.0. 
Meanwhile, <allow-navigation href="*"/> is also needed in config.xml but it is not added 
<br>
Fix:
<br>
add the following code in Your-Project/platforms/ios/config.xml


<pre>
  <code class="ruby">
      <feature name="IntentAndNavigationFilter">
        <param name="ios-package" value="CDVIntentAndNavigationFilter"/>
        <param name="onload" value="true"/>
      </feature>
  </code>
</pre>


 <br>   
 add <allow-navigation href="*"/> in the config,,xml too if needed.
 
 
 <br>
Ref: 
https://groups.google.com/forum/#!searchin/phonegap/iframe$20not$20working|sort:date/phonegap/c7QX4LPP4Wc/pojm0t3mBAAJ
