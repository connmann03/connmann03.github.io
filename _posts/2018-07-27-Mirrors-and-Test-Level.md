---
layout: post
title: "Mirrors and Test Level!"
date: "2018-07-27"
projects: [Sneaking Game]
tags: [Sneaking Game, UE4, Programming, Multiplayer, Replication, Design, Level Design, Thief, Stealth]
excerpt: "Today's work involved making more things to make the game fun"
images: [[2018-07-27 Movable Handheld Mirror.png],[2018-07-27 Test Level.png]]
---

Today's work involved making more things to make the game fun, so first the bushes that you can pickup and attach to the player, the code was moved to the player and called on the server so it works 100% of the time, and since it just floats in the air depending on your Z value, I made it get a linetrace and on that linetrace it would snap to the nearest ground.

After getting this work, I made a mirror that you can rotate with right clicking and dragging the mouse and only then. It is held in the same hand as the phone and it looks really neat.

{% include image.html filename="2018-07-27 Movable Handheld Mirror.png" description="Movable Handheld Mirror" %}

After that I started making a test level that is to test what to add to the game and proof of concept.

{% include image.html filename="2018-07-27 Test Level.png" description="Test Level" %}