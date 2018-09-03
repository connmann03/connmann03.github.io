---
layout: post
title: "More Features"
date: "2018-07-26"
projects: [Sneaking Game]
tags: [Sneaking Game, UE4, Programming, Multiplayer, Replication, Bugs, Thief, Stealth, Troll]
excerpt: "Today's work involved making the cameras work on multiplayer and correctly replicate the movement to everybody."
images: [[2018-07-26 Soulja Boy Phone Troll.png],[2018-07-26 Client Controller Camera.png]]
---

Today's work involved making the cameras work on multiplayer and correctly replicate the movement to everybody. I got this working and then the spot lights also. I then was trying to get where the sneaking players could use their phone to obstruct the camera's picture and "troll" the home owner/security guy. I first spent a couple hours figuring out what was wrong but I moved the code to the character and instead of spawning an actor it already has a phone on the camera, it's just hidden on begin play then on certain events it makes the phone have the Soulja Boy image.

{% include image.html filename="2018-07-26 Soulja Boy Phone Troll.png" description="Soulja Boy Phone Troll" %}

{% include image.html filename="2018-07-26 Client Controller Camera.png" description="Client Controller Camera" %}

The second image is the client controller's camera and it's replicating to the server and other clients (which is good).