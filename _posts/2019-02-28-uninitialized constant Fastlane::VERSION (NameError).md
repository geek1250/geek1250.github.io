

---
layout: post
title:  "`ensure in take_off': uninitialized constant Fastlane::VERSION (NameError)"
subtitle: ""
categories: ""
author: Geek
date:   2019-02-28 15:54:56 -0400
background: '/img/posts/03.jpg'
---
Error:
<br>
[⠏] 🚀 /Users/YOURUSERNAME/.rvm/gems/ruby-2.3.3/gems/fastlane-2.116.1/fastlane/lib/fastlane/cli_tools_distributor.rb:122:in `ensure in take_off': uninitialized constant Fastlane::VERSION (NameError)
	from /Users/YOURUSERNAME/.rvm/gems/ruby-2.3.3/gems/fastlane-2.116.1/fastlane/lib/fastlane/cli_tools_distributor.rb:122:in `take_off'
	from /Users/YOURUSERNAME/.rvm/gems/ruby-2.3.3/gems/fastlane-2.116.1/bin/fastlane:23:in `<top (required)>'
	from /Users/YOURUSERNAME/.rvm/gems/ruby-2.3.3/bin/fastlane:23:in `load'
	from /Users/YOURUSERNAME/.rvm/gems/ruby-2.3.3/bin/fastlane:23:in `<main>'
	from /Users/YOURUSERNAME/.rvm/gems/ruby-2.3.3/bin/ruby_executable_hooks:24:in `eval'
	from /Users/YOURUSERNAME/.rvm/gems/ruby-2.3.3/bin/ruby_executable_hooks:24:in `<main>'

<p>
Fix steps(not sure which step finially work):
<br>
sudo gem install rubygems-update
<br>
gem update --system
<br>
fastlane
