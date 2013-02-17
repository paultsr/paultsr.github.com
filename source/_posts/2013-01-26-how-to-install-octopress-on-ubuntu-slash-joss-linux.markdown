---
layout: post
title: "How to install Octopress on Ubuntu / JOSS Linux"
date: 2013-01-26 00:52
comments: true
categories: [octopress, ubuntu, joss, linux, install, blog]
---
## Installation Steps 

( open up the terminal and paste the following commands one by one )

1. `cd`
2. `sudo apt-get install zlib1g-dev openssl libopenssl-ruby1.9.1 libssl-dev libruby1.9.1 libreadline-dev git-core`
3. `git clone git://github.com/sstephenson/rbenv.git .rbenv`
4. `echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc`
5. `echo 'eval "$(rbenv init -)"' >> ~/.bashrc`
6. `exec $SHELL`
7. `mkdir -p ~/.rbenv/plugins`
8. `cd ~/.rbenv/plugins`
9. `git clone git://github.com/sstephenson/ruby-build.git`
10. `cd ruby-build`
11. `sudo sh ./install.sh`
12. `rbenv install 1.9.3-p194`
13. `rbenv rehash`
14. `rbenv global 1.9.3-p194`
15. `cd`
16. `git clone git://github.com/imathis/octopress.git octopress`
17. `cd octopress`
18. `gem install bundler`
19. `rbenv rehash`
20. `bundle install`
21. `rake install`




License
-

Paul S

*Free Software!*  

*Tested in Ubuntu 11.10 and JOSS Linux 1.10.3*

