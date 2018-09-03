---
layout: post
title: "Broken Game"
date: "2018-07-17"
projects: [Mowing Game]
tags: [Mowing Game, UE4, Multiplayer, Playtesting, Battle Logic, Replication, Bugs, Programming]
excerpt: "Today's work was involving testing the gameplay and adding a way to fight the other players."
images: [[2018-07-17 Lobby Map Ramp and Battle Projectile.png]]
---

Today's work was involving testing the gameplay and adding a way to fight the other players. I was able to add a test orb that attaches to the player on run over and then able to throw it and hit a player if it is at a certain velocity. But I forgot to add the durability below 0 detection, so you don't die after you get hit by a ball. I also added some ramps that launch the player (but are very buggy).

Play test bugs found; 
- if you become big and you die on clients you don't die on server
- replication isn't working for the death on clients/durability isn't being replicated correctly to the clients/server
- when you become big and you go into pool you're stuck infinitely
- if you die from the pool's damage you die infinitely
- shooting ball midair while moving forward will collide the shooter with ball
- ramps need to have more Z velocity
- balls don't detect after if person that was hit if they have 0 durability
- replication.

I have a lot to fix tomorrow, but it's mostly just replication bugs.

{% include image.html filename="2018-07-17 Lobby Map Ramp and Battle Projectile.png" description="Lobby Map Ramp and Battle Projectile" %}