---
layout: post
title: "Run Windows applications on Linux"
date: 2013-02-14 16:33
comments: true
categories: [ubuntu,linux,joss,windows,wine,emulator,applications] 
---
##Wine Doors 0.1 & Wine in Ubuntu

Wine Doors is an application that allows easy installation and managing of Windows application on Linux desktop .

This what Wine Doors Website has to say : -

Wine-doors is an application designed to make installing windows software on Linux, Solaris or other Unix systems easier. Wine-doors is essentially a *package management tool* for windows software on Linux systems.

Since Wine-Doors is basically to manage applications installed through wine and simplify their installation through wine so installing wine is a must.

**To install Wine** 

`sudo apt-get install wine`

After installing wine click *here* to download the latest version of Wine-Doors(*wine-doors_0.1.3rc1_all.deb*)

Install the following packages from a terminal

`sudo apt-get install orange`

`sudo apt-get install cabextract`

`sudo dpkg -i wine-doors_0.1.3rc1_all.deb`

I have used wine-doors release candidate 1 .

After completing above steps launch Wine-Doors from **Applications -> System-Tools -> Wine-Doors**

Now Wine-Doors would download and install some necessary apps and when all this inital confiuguration is over you would find a dialog like this providing you a easy way of installing a number of popular windows application.

I Was highly impressed by the ease with which it is possible to install many popular application using wine-doors.It was really impressive .There are a lot of windows applications that can be installed by wine.Check the *wine site* for the new windows applications which it supports.

{% img center /images/wine-doors1.png wine installation on linux image1 %}

{% img center /images/wine-doors3.png wine installation on linux image2 %}

*Wine-Doors in Action*

License
-

Paul S

*Free Software Supporter!*

*Tested in Ubuntu and JOSS Linux*
