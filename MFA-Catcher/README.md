# MFA Catcher

This project allows Tasker to detect and forward MFA codes from my phone to wherever I want.

## Problem 
When you're on your PC all day and keep needing to go back to your phone to input MFA codes and one-time passwords that are sent by online services via SMS. I wnated to solve this hassle of switching between devices. 

Now I know there are services that sync messages between your phone and PC, but they're not "smart". I didn't want all my messages on my PC, and having to look through the most recent one, and copy the code. Too much work. 

## Solution 
The solution is two-fold. 
 1. Detect a relevant MFA code being received. 

 This is easy. I use a filter to detect messages from only identified senders. For example, my bank, Amazon, etc. Next, I use regex matching to see if the message received contains a 6-digit number. If so, I extract it, and I now have my MFA code. 

 2. Send the code to my PC or another device. 

 * Tasker has a plugin called [Join](https://joaoapps.com/join/). This can be installed on a PC as a Chrome extension. 
 I use Join to push the code from my phone to my PC's clipboard. Yes, all that is needed to be done on the PC is a Ctrl+V, and voila. 

 * I also use Tasker to send this MFA code to a private Telegram channel using the [Telegram Bot API](https://core.telegram.org/bots). Now I can access this code from my Tablet as well or with other people if I wanted to.

 ## Implementation 

One-time password received on the phone triggers this profile. 
<img src = "https://user-images.githubusercontent.com/85018020/147509050-31ce848c-8b6f-4c8b-9dda-95c0a1042115.png" width = 40% />

Tasker extracts the 6-digit code and sends it to the Telegram Channel and puts it on my clipboard on my PC. 

<img src = "https://user-images.githubusercontent.com/85018020/147509080-c801a48d-5587-49bd-8bd6-89f277896b0c.png" width = 40% />

## Installation

You can import my profile as an XML file in Tasker. Go to the overflow menu, select import, and choose the xml file in this repository (downloaded to your phone). 
