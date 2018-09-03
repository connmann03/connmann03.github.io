---
layout: post
title: "Adding Land Lots & Arrows"
date: "2018-07-11"
projects: [Mowing Game]
tags: [Mowing Game, UE4, Technical Artistry, Bugs, Crazy Taxi, 2001 A Space Odyssey, Film]
excerpt: "Today's work started off smooth, I finished the grass spawning volume and it randomly spawned within the volume's boundaries."
images: [[2018-07-11 Crazy Taxi Arrow.png,"Crazy Taxi Arrow"],[2018-07-11 Crazy Taxi Arrow Moving.png,"Crazy Taxi Arrow Moving"]]
---

Today's work started off smooth, I finished the grass spawning volume and it randomly spawned within the volume's boundaries. I then made a Crazy Taxi style arrow that would pop up over a "lot" of land. This arrow had a moving striped pattern and has a background and stripe color I can change as parameters. I then made it go up and down and rotate in a spiral looping. After this, I attached the arrow in the world to the grass spawners in a lot. The arrow is the parent. The code worked and it successfully attached and I was able to get a reference to the spawners attached in the arrow's blueprint and assign it to variables. But, after this I was trying to get the grass that was attached to the spawner to be in this structure as it's called in Unreal Engine 4. A structure is a group of variables and in the arrow blueprint I have a variable that is an array of this structure. The structure has a spawner reference and an array of grass for each spawner. I tried to get all of the attached grass pieces from inside the arrow and it kept returning null. I tried everything and in the world, if I select the spawner, it highlights the grass pieces, which is correct. Then after toying around, Austin tried to help find a solution. It was almost working but when we executed it, it crashed. Then we removed the code we added, and it kept crashing. I later found out I guess the "Add Child Actor Component" node crashes. It NEVER crashed until now. I've also used this sort of node in August 2017, and it never crashed. It was also in this usage of spawning many, many actors. 
Also, earlier today I got to see 2001: A Space Odyssey in 70mm at AFI: Silver Springs. It was amazing. But I still need to solve that bug. I assume it's an editor bug...like always.

{% include image.html filename="2018-07-11 Crazy Taxi Arrow.png" description="Crazy Taxi Arrow" %}

{% include image.html filename="2018-07-11 Crazy Taxi Arrow Moving.png" description="Crazy Taxi Arrow Moving" %}

{% include youtubePlayer.html id="oR_e9y-bka0" %}