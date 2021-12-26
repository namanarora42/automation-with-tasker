# Missed Call Alert

We live in a world where we are constantly at risk of getting distracted by our phones. Often times, you might want to silence your phone and get disconnected, whether it is for a meeting, or just taking a break. How many times have you fogotten taking your phone off silent, or missed an extremely urgent phone call that you could have justified a distraction for? 

## Problem 

In the metaverse that we are moving towards, being unavailable to take an urgent could very well be a life or death situation. I created this project after getting my parents worried about my well being, as I had slept off during the day with my phone on silent, and no way for them to contact me. 

## Solution

First off, I can choose to identify "special callers" or treat all callers as equal. In my current setup, the script triggers only if the repeat caller is a special caller, such as close friends and family. 

For a repeat caller, I would want them to know that my phone is on silent and I'm unable to hear it. If they still want to go ahead with their call, I want to allow them, and provide them a way to "break" the silence of my phone. After every missed call, I track all missed calls for the next 10 minutes. This tracking can be aborted if I need to. 

Tracking started: 

<img src = "https://user-images.githubusercontent.com/85018020/147400168-ffa939ab-340f-4d5c-a1ff-9ef6be398497.jpg" width = 40%/>

After the second phone goes unanswered from the same caller (thus getting 2 missed calls), Tasker sends an automated response to the caller. 

Automated Response Sent to Caller:

<img src = "https://user-images.githubusercontent.com/85018020/147400171-a6601eac-ab32-4eb0-a5af-eaa21d8d1e2d.jpg" width = 40%/>

If the caller still wishes to break the silence and make my phone ring, they will call again. And this time if I don't answer, my phone will come out of "Silent" mode and start ringing, thus waking me up/alerting me of the urgency. 

<img src = "https://user-images.githubusercontent.com/85018020/147400193-dace30bb-8e57-4912-9500-3dd49fdd6772.jpg" width = 40%/>

It starts playing media in full screen and shows a button that will disable the disable the ringer. 

## Installation

You can import my profile as an XML file in Tasker. Go to the overflow menu, select import, and choose the xml file in this repository (downloaded to your phone). 