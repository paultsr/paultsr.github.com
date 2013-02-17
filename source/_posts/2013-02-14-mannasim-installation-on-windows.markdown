---
layout: post
title: "Mannasim Installation on Windows"
date: 2013-02-14 10:52
comments: true
categories: [ns2,mannasim,windows,joss,windows7,windowsxp,windows vista,windows8,sensor,networks,wireless,simulator]
---
More than half of my pg mates are doing their project work in sensor networks.I had seen my friends struggling to install Mannasim on their laptops.But, iam doing my project on Grid Security. So i thought to write a blog for my friends who all are keen to simulate WSN.

Mannasim is a module which extends NS2 to simulate different Wireless Sensor Networks (WSN) applications.
I had patched the NS2.29 with mannasim module and is available *here*.I had installed it in my Vista OS.It will also work in Windows XP.

## Installation Steps  

Before installing mannasim, you should install cygwin.You can check my *previous post* for cygwin installation.After installing cygwin, install the ns2.29 as described in the same post.The only difference is the ns2 version which we are using here is ns-allinone-mannasim-2.29.tbz.

After installing mannasim, copy the ns2.sh file to */etc/profile.d* folder

`cp /usr/local/ns-allinone-2.29/paulson/.set/ns2.sh /etc/profile.d/.`

Then type the following command in the terminal

`source /etc/profile.d/ns2.sh`

You can find the sample codes in the folder

*C:\cygwin\usr\local\ns-allinone-2.29\paulson\sample-codes\mannasim*

**Mannasim Script Generator(MSG)** comes with the mannasim module.It can be used to create ns2 simulation scripts(.tcl) easily and that too with a gui interface.It is very simple to use.You can find the tool in the folder

*C:\cygwin\usr\local\ns-allinone-2.29\ns-2.29\mannasim\scriptGeneratorTool*

Double click the *msg-win32* batch file.
or
type the following command in the cygwin terminal

`cd /usr/local/ns-allinone-2.29/ns-2.29/mannasim/scriptGeneratorTool/
./msg-linux.sh`

some screen shots are given below : 

{% img center /images/ns2-mannasim2.jpg mannasim installation on windows image1 %}
{% img center /images/ns2-mannasim4.jpg mannasim installation on windows image2 %}
{% img center /images/ns2-mannasim5.jpg mannasim installation on windows image5 %}

*NOTE : For any installation problems, read the comments for this blog.*

License
-

Paul S

*Free Software Supporter!*

*Tested in Windows XP, Windows Vista SP1 and Windows 7*

