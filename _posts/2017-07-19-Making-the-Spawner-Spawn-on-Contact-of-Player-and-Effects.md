---
layout: post
title: "Making the Spawner Spawn on Contact of Player and Effects"
date: "2017-07-19T16:11:58+05:30"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Gauntlet, Level Design, Programming Fundamentals, Controls, Lord of the Rings, Travel, Bugs, Lighting, Particle Systems]
excerpt: "Sorry for the long wait, we were all on a trip in Japan. It was fun but now we work."
images: [[portal.png],[flash.png]]
---

Sorry for the long wait, we were all on a trip in Japan. It was fun but now we work. Today's work involved working on getting the spawner fixed again (since it broke for some reason) and adding effects to it. I solved the spawner situation with my brothers since they thought the troll wasn't spawning since it was too big, so we moved the arch back and it spawned. After that, I began adding effects to the spawner. 

I thought of the spawner as a sort of "portal" since it's an archway I thought of it that way. What I did next was add an effect to the archway that was a portal spiral. Then I added a glow from a spotlight that shot upwards in the air and was super bright, like a greenish blue. Next, I added a point light that made it glow more. After that, I tweaked a smoke particle and made it emit on the ground as a greenish color for that "portal feeling".

Next, I made it so when the enemies spawn they have a spark particle as they're being beamed in. I then finished with a destruction particle of the spawner.

{% include image.html filename="portal.png" description="Portal" %}

{% include image.html filename="flash.png" description="Flash" %}