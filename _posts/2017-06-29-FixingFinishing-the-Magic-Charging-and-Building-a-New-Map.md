---
layout: post
title: "Fixing/Finishing the Magic Charging and Building a New Map"
date: "2017-06-29T23:55:00-05:00"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Gauntlet, Animation, Level Design, Programming Fundamentals, Controls, Lord of the Rings]
excerpt: "Today's work involved figuring out how to get the magic charging ability to work and after that building a map."
images: [[outside.png],[wal.png],[entrance.png],[dropoff.png],[ramp.png],[walkway.png],[staircasedrop.png],[staircasedown.png]]
---

Today's work involved figuring out how to get the magic charging ability to work and after that building a map. I started with the magic charging. What I was trying to do was change the particle on the fly in the KGProjectileBase, which holds the projectile (magic), if the player is charging up during certain intervals. I had it so it would work if less than 2 seconds but it wasn't a particle change. It was just changing the animation montage as a test and that worked. So, I got stuck so Austin helped me and he figured out that if you make a variable in the player controller, where the charging happens, of a particle system and set that on different charge intervals it works. The only thing you have to add is adding a cast to the player controller in the projectile and get the variable we made in there and set it to the particle system in KGProjectileBase.

After Austin helped me, he told me to get inspiration from LOTR, Harry Potter, and Gauntlet Legends. So, I opened three windows and put them on my screen with images and videos that best fit what would look good. Next, I drew a design and started building. This is what I came up with:

{% include image.html filename="outside.png" description="Outside" %}
{% include image.html filename="wal.png" description="Doorway" %}
{% include image.html filename="entrance.png" description="Entrance" %}
{% include image.html filename="dropoff.png" description="Dropoff" %}
{% include image.html filename="ramp.png" description="Ramp" %}
{% include image.html filename="walkway.png" description="Walkway" %}
{% include image.html filename="staircasedrop.png" description="Staircase Dropoff" %}
{% include image.html filename="staircasedown.png" description="Staircase Down" %}

I built the castle-like a LOTR castle. I took me a couple hours of off-and-on working with breaks since it's a pain to move that amount of meshes and perfectly align them. But, tomorrow I will finish it.