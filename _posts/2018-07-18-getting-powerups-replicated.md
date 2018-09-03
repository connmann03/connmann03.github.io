---
layout: post
title: "Getting Powerups Replicated!"
date: "2018-07-18"
projects: [Mowing Game]
tags: [Mowing Game, UE4, Multiplayer, Playtesting, Battle Logic, Replication, Bugs, Programming]
excerpt: "This morning, I started bug fixing and I made the powerups spawn on the Player State and then the events run on the server!"
images: [[2018-07-18 Projectile Arc.png],[2018-07-18 Durability Bug.png]]
---

This morning, I started bug fixing and I made the powerups spawn on the Player State and then the events run on the server! This half way worked, then I remembered, I didn't replicate the powerup type variable. It then worked 100% of the time.

This afternoon, I was working on fixing the powerups replicating, and I got it to work. Then I added the ball to arch and show the arc. 

After most of the day trying to get the arch and stuff, I got it to work and packaged it and Austin and I tested it. We figured out that the durability wasn't correctly being replicated.

{% include image.html filename="2018-07-18 Projectile Arc.png" description="Projectile Arc" %}

{% include image.html filename="2018-07-18 Durability Bug.png" description="Durability Bug" %}