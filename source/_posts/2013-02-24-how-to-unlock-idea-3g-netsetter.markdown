---
layout: post
title: "How to Unlock Idea 3G Netsetter"
date: 2013-02-24 11:59
comments: true
categories: [hacking,Idea,mobile,3g,Netsetter,tech,unlock]
description: "How to Unlock Idea 3G Netsetter"
keywords: "hacking,Idea,mobile,3g,Netsetter,tech,unlock"
---

##STEP BY STEP GUIDE TO UNLOCK IDEA 3G NETSETTER

{% img center /images/idea_unlock/netsetter.png unlock idea 3g netsetter image0 %}

1) Download the cdma workshop and download huawei e1732 downgrader ( disable antivirus before opening the cdma workshop ).

[cdma workshop free download](http://cesa.co.in/downloads/idea/CESA_1.zip)

[huawei e1732 downgrader free download](http://cesa.co.in/downloads/idea/CESA_2.zip)

2) Insert a non idea sim to your Idea 3G Netsetter (e1732 ).

3) Find the common port to which your Idea 3G Netsetter (e1732 ) modem is connected.

**Right click on your My Computer icon > Properties > Device Manager > Ports (COM & LPT)  > HUAWEI Mobile Connect – 3G Application Interface (COM [The port number appear in your system] )**

4) Run *CDMA Workshop v2.7.0.exe*

5) Select the Port that you noted from your Device Manager under the Port option in *COM Settings (AT mode)* under the *Main* tab.

6) Then click on *connect* and then click on *read*

{% img center /images/idea_unlock/1.jpg unlock idea 3g netsetter image1 %}

<!-- more -->

7) Go to the *Security* tab > Type *000000* in the blank box under *SPC* > Click on *SPC* button > Click on *Send* with Default (*nv_read*) as SPC.

{% img center /images/idea_unlock/2.jpg unlock idea 3g netsetter image2 %}

8) Click on *Memory* tab > *NV Items* > *Read* > Now a *Conform* box will appear > Click *OK* > Now a *NV Items Backup* box will appear > In the box straight to *Last NV Item* type *9999* > Click *OK* > Save the file by giving a file name you like (Eg: [E1732Unlock](http://cesa.co.in/downloads/idea/CESA_5_E1732Unlocker.txt))

{% img center /images/idea_unlock/3.jpg unlock idea 3g netsetter image3 %}

9) When the buffer reach *100%* your file is saved successfully. Now a *Information* box will appear > Click *OK* > Minimise *CDMA Workshop v2.7.0*

10) Run *E1732 Downgrader8 >  *accept* the agreement > *Next* > Wait for a few seconds until the search for your modem finishes > (Don’t mark on *Auto remove the device after update*) *Next* > (Don’t remove your data card until the process is finished) > *Start* > At the end of *Downloading Programs…* you will get a *Update Failure!* error dialog box (DON’T WORRY & DON’T GET DISAPPOINTED) > Click *OK* > Click *Finish*

11) Restore *CDMA Workshop v2.7.0* > *Main* tab > *Disconnect*

12) Unplug your Idea 3G Netsetter (e1732 ) modem from your computer.

13) Again Plug it to the Computer. Check the *Port* again from the *Device Manager*

14) Go to *CDMA Workshop v2.7.08 select the Port that you noted from your Device Manager under the Port option in *COM Settings (AT mode)* under the *Main* tab as we did before > Click on *Connect* > *Memory* tab > *NV Items* > Click on *Write* > A *Confirm* box will appear > Click *OK* > *Open* dialog box will appear > Open the file that you saved before > When the buffer reach *100%* a *Information* dialog box appears with a success message > Click *OK* > *Main* tab > *Disconnect*

15) Now close *CDMA Workshop v2.7.0* > A *Confirm* dialogue box will appear > Click *NO*

16) Close everything and Enable your Antivirus

17) That’s it. Your Idea 3G Netsetter (e1732 )is unlocked successfully.

18) Unplug Idea Netsetter (Modem) from your computer.

19) Put a SIM Card other than IDEA to the Netsetter and again Plug it to the Computer.

20) Wait for Idea Netsetter to Start. It will detect the SIM card and enjoy browsing with any other SIM.

**To make new mobile apn settings you can download huawei mobile partner**

[Mobile Partner free download](http://cesa.co.in/downloads/idea/CESA_3.zip)

Many people are having problem while connecting to internet with other sim cards now you can connect by any sim card with default IDEA net Setter Dashboard using these steps. If your Modem is detecting sim cards and you are getting errors then try this

**Windows XP**

Open *Control Panel* -> *Phone and Modem* (found directly in control panel or in *Printers and other hardware* ) –> *modem* tab –> *huawei mobile connect 3g modem* (which is present on COM ) –> *properties advance* –> *extra initializing command* use given commands below and click *OK*

**Windows 7**

In the start menu, type *phone and modem* — *click* on itb —> *modems* –> *huawei mobile connect 3g modem* –> *properties* –> *change settings* –> *advance* –> *extra initialization command* –> use given commands below and if it asks for Country and area code then set Country to *India* and Area Code to *91* and leave other fields blank.

**commands/settings**

**Aircel** : `AT+CGDCONT=1,"IP",”aircelgprs”`

**Airtel** : `AT+CGDCONT=1,”IP”,”airtelgprs.com”`

**BSNL** – `AT+CGDCONT=1,”IP”,”bsnlnet”`

**Idea** – `AT+CGDCONT=1,”IP”,”internet”`

**Reliance** – `AT+CGDCONT=1,”IP”,”rcomnet”`

**Tata Docomo** – `AT+CGDCONT=1,”IP”,”tata.docomo.internet”`

**Videocon** – `AT+CGDCONT=1,”IP”,”vinternet.com”`

**Vodafone** – `AT+CGDCONT=1,”IP”,”www”`

 *If you have any trouble doing this please comment here*

License
-

Paul S

*Free Software Supporter!*

*Tested in Windows XP, Windows Vista SP1 and Windows 7*










