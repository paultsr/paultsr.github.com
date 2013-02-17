---
layout: post
title: "MAC ID Spoofing"
date: 2013-02-14 11:27
comments: true
categories: [macid,linux,ubuntu,hacking,tweaks,tips,spoofing,hardware address,joss linux]
---
To change the mac id of your network interface card in Linux, you hav to edit  */etc/rc.local* file.If the file rc.local is not present in the */etc* directory, create a new file of the same name.

Open the *rc.local* file in a terminal :-

`sudo gedit /etc/rc.local`

Then add the following lines before *exit 0* line:-

`/etc/init.d/networking stop`

`ifconfig eth0 hw ether xx:xx:xx:xx:xx:xx`

`/etc/init.d/networking start`

Save the file and Restart the machine.Now you mac id will be the new mac id you had assigned.To verify, type the following command in a terminal

`ifconfig`
