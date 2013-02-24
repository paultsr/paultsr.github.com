---
layout: post
title: "How to install Octopress on Ubuntu / JOSS Linux"
date: 2013-01-26 00:52
comments: true
categories: [octopress, ubuntu, joss, linux, install, blog]
description: "How to install Octopress on Ubuntu"
keywords: "octopress, ubuntu, joss, linux, install, blog"
---
## Installation Steps 

( open up the terminal and paste the following commands one by one )

```  
$ cd
$ sudo apt-get install zlib1g-dev openssl libopenssl-ruby1.9.1 libssl-dev libruby1.9.1 libreadline-dev git-core
$ git clone git://github.com/sstephenson/rbenv.git .rbenv
$ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
$ echo 'eval "$(rbenv init -)"' >> ~/.bashrc
$ exec $SHELL
$ mkdir -p ~/.rbenv/plugins
$ cd ~/.rbenv/plugins
$ git clone git://github.com/sstephenson/ruby-build.git
$ cd ruby-build
$ sudo sh ./install.sh
$ rbenv install 1.9.3-p194
$ rbenv rehash
$ rbenv global 1.9.3-p194
$ cd
$ git clone git://github.com/imathis/octopress.git octopress
$ cd octopress
$ gem install bundler
$ rbenv rehash
$ bundle install
$ rake install
```  

License
-

Paul S

*Free Software!*  

*Tested in Ubuntu 11.10 and JOSS Linux 1.10.3*

