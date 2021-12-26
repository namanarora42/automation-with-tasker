# Smarter Alarm Clock

Alarm clock applications on smartphones just work. They don't do much of "smart", but they work. 

There are certainly some "tougher" alarm clock apps available that might make you do some math, take a picture, or scan an NFC tag to make the alarm stop blaring, hence guaranteeing that you don't go back to sleep. 

## **Problem**

My problem with these third party apps has been the inability to dismiss an alarm the normal way. Sometimes I would be certain of being wide awake and not need to solve a complex math problem for no reason. Sometimes I would want to set an alarm for not waking up at all. I might be using it as a reminder for some task. Wouldn't wanna scan any NFC tags then. 

## **Solution**

My solution was simple. The app needs to present a mini-challenge that is easily solvable. If I don't solve that mini-challenge within a particular time window (during which I can either doze back off to sleep or become wide awake), then a harder main challenge pops up and the alarm starts going off again. 

## **Implementation**

### _The Mini Challenge_
Once the alarm goes off, and I dismiss it, Tasker sends a notification to my shade. It just notifies of the challange being initiated and a button to abort it. If I press abort, then that's it. The script assumes I'm wide awake and no further challanges will be thrown. 

However, if I don't press Abort within 10 minutes, the script assumes that I've dozed off again and it's time to bring out the big guns.

### _The Main Challange_
10 Minutes have passed since I dismissed that alarm but didn't abort the mini challange. The room is silent. And now, the alarm fires for a second time, on its own. This time I am presented with a challange. I had to read out a phrase from the screen and type it in as-is. I could have made this harder, but this works just fine for me. Once I key in the phrase, the alarm is dismissed. The alarm tone stops playing, and I am certainly wide awake.

## **Installation**

You can import my project as an XML file in Tasker. Long press on the bottom navigation bar, select import, and choose the xml file in this repository (downlaoded to your phone). 

## **Demo**



https://user-images.githubusercontent.com/85018020/147399275-faf479b5-92df-40d1-a820-64621c2ed90f.mp4

