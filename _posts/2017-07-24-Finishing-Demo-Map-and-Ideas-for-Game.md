---
layout: post
title: "Finishing Demo Map and Ideas for Game"
date: "2017-07-24T16:11:58+05:30"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Gauntlet, Enemy Design, Hexen, NavMeshes, AI, Level Design, Brainstorming, Controls, Dealing Damage]
excerpt: "Today's work involved finishing the demo area and coming up ideas for the next concepts to implement into our game."
images: [[bigroom.png],[dropoff2.png],[spiral.png],[aimingup.png],[shoot.png]]
---

Today's work involved finishing the demo area and coming up with ideas for the next concepts to implement into our game. I first started creating the rooms and finishing them. Then, I had the idea to have enemies drop off a wall that you can't get too (and potentially not see) and attack you. Then, Adam said there are things called Nav Mesh Proxies that allow you to have AI drop off ledges and jump to ledges just based the position you place the points. This worked instantly after we messed with the radius of where the AI can interact with the point with. I then added all the spawners to the level and implemented the timings correctly.

{% include image.html filename="bigroom.png" description="Big Room" %}

{% include image.html filename="dropoff2.png" description="Enemy Drop In Nav Mesh Prox" %}

{% include image.html filename="spiral.png" description="Spawner to Spiral Staircase Nav Mesh" %}

After that, Austin fixed the projectiles so they hurt the new enemies. Next, Austin made the arrow move up and down with your mouse. This worked instantly since the arrow is where the projectiles come out of. 

{% include image.html filename="aimingup.png" description="Aiming Up" %}

{% include image.html filename="shoot.png" description="Shooting Projectile While Aiming Up" %}

Also, I was told to think of concepts, so here are my ideas:

- More enemies
- Fix damage for projectiles so each projectile has different damage
- Finish the map by fixing the lighting
- Making a randomized drop system with a way to pick them up and have an inventory for the player
- Multiplayer
- Destruction timer for projectiles
- Fix spawner to detect projectile 
- Repetitive attack when Mouse1 held down
- Magic attacks that are like fire walls, lightning strikes need to stay for a certain 
- Fix damage for attacking
- Make spawners invisible then in a trigger volume make them appear
- Limit to spawning
- Make spawners not spawn so fast
- Center the mouse/camera and arrow needs to face it
- If not in radius of player, AI needs to make wall around player
- AI Swarming player to surround the player (making it harder)
- Make floating worm float above trolls and fly over
