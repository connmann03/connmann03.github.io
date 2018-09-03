---
layout: post
title: "Navigation and Expansion"
date: "2018-07-12"
projects: [Mowing Game]
tags: [Mowing Game, UE4, 3D Modeling, Blender, AI, NavMesh, Bugs, Tony Hawk's Pro Skater, Level Design, Programming]
excerpt: "Last night's bug was solved after I wrote my post, Austin insisted we solve it."
images: [[2018-07-12 Car AI Nav Meshes.png],[2018-07-12 Car AI Nav Meshes Ramp.png]]
---

Last night's bug was solved after I wrote my post, Austin insisted we solve it. After that I went to bed and then the next morning I made a car model in Blender. I learned more about modeling while making it. I started off with a cube and a circle. The circle wasn't 3D so I was able to copy the edges and paste them a certain amount of units away and make a 3D circle. This then turned into a semi-circle that was put on top of the cube(body of the car) as a windshield. Then I made 4 semi-circles that were 2D as wheels.

{% include image.html filename="2018-07-12 Car AI Nav Meshes.png" description="Car AI Nav Meshes" %}

I then made an AICar class that had the model and moved to different target points around the map and automatically follows and loops. It is really awesome since it automatically turns the car so I don't have to manually make a turning function(I tried that before the AI test). I then expanded the map some more and made the Arrow change colors after the lot being completely mowed to the player's randomly generated color.

{% include image.html filename="2018-07-12 Car AI Nav Meshes Ramp.png" description="Car AI Nav Meshes Ramp" %}

Also, I added skitching where you grab onto the back of a car. You hold down space before you are about to approach the car, and you attach. You keep holding down space until you want to stop and let go.

{% include youtubePlayer.html id="ttuW2ab57uM" %}
