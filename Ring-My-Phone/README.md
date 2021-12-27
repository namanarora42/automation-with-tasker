# Ring (Find) My Phone 

> If you came here expecting a project that lets you get the GPS coordinates of your phone, [this](https://github.com/namanarora97/automation-with-tasker/tree/main/SOS-Location) is the project for you.

This project is another implementation of SMS-driven events. I thought of this idea when I had lost my phone while at a party, and my phone, _obviously_, was on vibrate-only. 

## Problem

The only way to make your phone ring once you lose it:
* Pray that it has an internet connection.
* Find a nearby computer or a friend's phone which also has an internet connection. 
* Login to your Google account.
* Your Google account is protected by MFA and _you need your phone to login_. 
* Cry eternally.

## Solution 

This should be very simple! Even if your phone doesn't have internet connectivity, it just needs a little bit of cellular service to be able to receive SMS. 

So what do I do? I grab my friend's phone, send myself this text:

<img src = "https://user-images.githubusercontent.com/85018020/147417468-1c41d9c3-ec63-4729-9d4e-4134d9786a75.png" width=40%/>

>#lost5678

And voila, wherever my phone is, internet or not, it will start blasting loud music, with this screen popped up:

<img src = "https://user-images.githubusercontent.com/85018020/147417444-123e6cd1-3248-4a56-9d9c-f53d11c4f1ae.jpg" width=40%/>



## Installation

You can import my profile as an XML file in Tasker. Go to the overflow menu, select import, and choose the xml file in this repository (downloaded to your phone). 
