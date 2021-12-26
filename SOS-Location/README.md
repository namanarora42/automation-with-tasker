# SOS Location Sharing

## Problem

I tried to solve two problems using this project. 
1. You lost your phone. It is on silent. You're not near a computer to be able to login to your Google account and do the Find My Phone stuff. 
2. Your loved ones cannot reach you. Your calls are going unanswered. These are people you trust and care about. They want to know where you are and if you are safe. 

## Solution

Upon receiving a unique "passphrase" via SMS, Tasker initiates a location share. It will reply back to the original sender with precise GPS coordinates of my phone along with the current battery percentage. 

This can be further enhanced by also capturing a photo from the front and back camera, and sharing a Google Drive link to those photos as a reply to that SMS. 

## Implementation 

My passphrase is : _#location5678_ 

As soon as anybody sends me that text message, Tasker sends a response with my current GPS coordinates, a Google Maps link, the accuracy (in meters) and the battery percentage.

![image](https://user-images.githubusercontent.com/85018020/147416780-a22e5964-e0a3-4f25-89c9-a40eef0e9da2.png)
