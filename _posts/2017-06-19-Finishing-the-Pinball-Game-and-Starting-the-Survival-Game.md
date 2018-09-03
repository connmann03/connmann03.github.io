---
layout: post
title: "Finishing the Pinball Game & Starting the Survival Game"
date: "2017-06-19T16:11:58+05:30"
projects: [Pinball Game, Horde Survival Game]
tags: [Learning, Courses, Game Design Fundamentals, UE4, Decals, Particle Systems, Terrain]
excerpt: "Today, I finished my pinball game."
---

Things I learned today:

- Decals
- Scale boxes
- UI Animations
- Particle Spherical Explosion Effect
- Particle Stuff
- Importing Assets from the Marketplace 
- Terrain

Today, I finished my pinball game. My final additions to the game were animations in the UI so the logo we added faded in getting bigger then bounced in and out, and also decals. And adding a shadow/shadow offset to the play button. Also, adding a free font we imported as the menu font and high scores list. Next, we made a texture a decal by putting it in a material and applying it to a decal on the level. Then, we made a particle system that when the bumper got hit by a ball, sparks went flying out of the bumper hitting objects on the table, colliding with them.

The way we did this was take a new particle system we created, add a sphere component, and then disable positive z and negative z values to make a flat circle. Then you would have to disable outer pace so it would make a ring. Then we made it shoot out like sparks in random times and random speeds in that ring pattern. Next, we needed a model for the spark so we made a material and made it have a flat spot that was transparent so you can make it different colors and brighter. We applied that to the particle system and changed the color to a orangish and it looks amazing so we added it in the Bump function and made it not loop. We finished the game.

I started the next game, a survival game, and I started the second video, terrain tools.