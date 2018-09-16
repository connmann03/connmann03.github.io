---
layout: post
title: "Spraypainting!"
date: "2018-08-26"
projects: [Sneaking Game]
tags: [Sneaking Game, UE4, Programming, Multiplayer, Replication, Design, Thief, Stealth, HUD, 3D Modeling, Blender, Gimp, Scoring]
excerpt: "Making the Spray Paint Can able to spray and make a decal on the wall."
images: [[spraypainting.PNG,Spray Painting In Action]]
---

Today's work involved getting spray painting to work and I did! Instead of using render targets I decided to use decals of a simple radial gradient exponential that is just a simple circle material built in and used it as a decal. The radial gradient exponential is a node inside the material editor. But, I made the player(for now) have a spray paint can automatically on them and has to pull it out like the mirror or phone. And the can you have to click over and over to spray paint so I have to make a holding mechanic to spray automatically over and over.

{% include image.html filename="spraypainting.PNG" description="Spray Can Model" %}