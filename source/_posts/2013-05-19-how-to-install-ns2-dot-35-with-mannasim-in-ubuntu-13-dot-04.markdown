---
layout: post
title: "How to install NS2.35 with Mannasim in Ubuntu 13.04"
date: 2013-05-19 23:20
comments: true
categories: [ns2, ns2.35, mannasim, linux, ubuntu, simulation, network, wireless, joss]
description: "How to install NS2.35 with Mannasim in Ubuntu 13.04/ Linux"
keywords: "ns2, ns2.35, mannasim, linux, ubuntu, simulation, network, wireless, joss"
---
## Installation Steps  
( open up the terminal and paste the following commands one by one )

1. `cd`
2. `sudo apt-get install zlib1g-dev openssl libopenssl-ruby1.9.1 libssl-dev libruby1.9.1 libreadline-dev git-core`
3. `cd /usr/local/`
4. `sudo git clone git://github.com/paultsr/ns-allinone-2.35.git`
5. `cd ns-allinone-2.35/`
6. `sudo ./install`
7. `source /etc/profile.d/ns2.sh`

Screen Shots

{% img center /images/mannasim/ns1.png ns2.35 with mannasim installation on ubuntu13.04 image1 %}
{% img center /images/mannasim/ns2.png ns2.35 with mannasim installation on ubuntu13.04 image2 %}
{% img center /images/mannasim/ns3.png ns2.35 with mannasim installation on ubuntu13.04 image3 %}
{% img center /images/mannasim/ns4.png ns2.35 with mannasim installation on ubuntu13.04 image4 %}
{% img center /images/mannasim/ns5.png ns2.35 with mannasim installation on ubuntu13.04 image5 %}
{% img center /images/mannasim/ns6.png ns2.35 with mannasim installation on ubuntu13.04 image6 %}
{% img center /images/mannasim/ns7.png ns2.35 with mannasim installation on ubuntu13.04 image7 %}
{% img center /images/mannasim/ns8.png ns2.35 with mannasim installation on ubuntu13.04 image8 %}
{% img center /images/mannasim/ns9.png ns2.35 with mannasim installation on ubuntu13.04 image9 %}
{% img center /images/mannasim/ns10.png ns2.35 with mannasim installation on ubuntu13.04 image10 %}


License
-

Paul S
*Free Software!*  

*Tested in Ubuntu 13.04 and JOSS Linux 1.10.3*
