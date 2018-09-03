---
layout: post
title: "Multiplayer Features"
date: "2018-07-24"
projects: [Sneaking Game]
tags: [Sneaking Game, UE4, Programming, Multiplayer, Replication, Bugs, Thief, Stealth, Design]
excerpt: "Today's work involved adding lights the security guy can turn on and off."
images: [[2018-07-24 Security Camera Controlled Spot Lights.png]]
---

Today's work involved adding lights the security guy can turn on and off. This worked, then after that I started replication of variables and actors like the screens, phones, movement, etc. I was able to get phones and cameras to replicate. But, I couldn't get the right pawn to possess after unpossession of the screen manager. I then came into another problem...The screens don't build after packaging the build. They're completely black.

{% include image.html filename="2018-07-24 Security Camera Controlled Spot Lights.png" description="Security Camera Controlled Spot Lights" %}