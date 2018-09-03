---
layout: post
title: "Messing With the Particle Editor and Adding a Charging Magic System"
date: "2017-06-28T16:11:58+05:30"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Gauntlet, Animation, Particle Systems, Controls]
excerpt: "Today's work involved messing with the particle editor to see what's possible in the editor and figuring out how to charge up your magic to result in a bigger magic ball."
images: [[beam.png],[ice.png],[charge.png]]
---

Today's work involved messing with the particle editor to see what's possible in the editor and figuring out how to charge up your magic to result in a bigger magic ball. I started messing with the particle editor. I decided it would be easier by starting out with the particle for the magic we already had. So, I duplicated it and I changed quite a few things. 

The things I changed were: lifetime, point gravity, sphere, spawn, color over life, etc. Messing with the sphere settings and disabling everything besides Positive and Negative Z made the particles emit in a light beam stream. Disabling the point gravity would make the particles fall down since there was a constant velocity of negative Z. Next, I changed the color of it so it was like a bright blue laser beam that glowed. Then I tried adding one particle ball that had the same point gravity properties, but it wasn't possible since it requires more particles.

{% include image.html filename="beam.png" description="Beam" %}

After messing with this beam, I made my own particle. This one was gonna be an actual ice beam since I started from scratch (so I know what I change). This one was just a simple spot material with a trail behind it in the Z axis. The particle had a constant velocity of positive Z. So, I made it big at the start of its life then super small at the end of its life so it was like an ice ball.

{% include image.html filename="ice.png" description="Ice Beam" %}

Next, I started messing with a charging system so you can charge your magic shot. I figured it out I need to get the amount of time the player holds down the button. Then I convert that to a variable and I reset and set it. This worked but I have to finish it tomorrow.

{% include image.html filename="charge.png" description="Magic Charge System Code" %}