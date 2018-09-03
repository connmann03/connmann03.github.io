---
layout: post
title: "Particles & More"
projects: [Apartment ArchViz Scene, Theater Room ArchViz Scene]
date: "2017-06-13T23:55:00-05:00"
tags: [Learning, Courses, Game Design Fundamentals, UE4, Particle Systems, Level Design]
excerpt: "Today's work involved finishing the last two videos of the visuals part of the Udemy course"
---

Today's work involved finishing the last two videos of the visuals part of the Udemy course, Unreal Engine 4: How to Develop Your First Two Games. The last two videos were titled, Finishing Touches (Part A/B), and it involved polishing the room we created. The first part of part A involved adding a particle system. Our particle system was made to look like dust was moving around the air. We did that by making the particles fade in to emit then fade out and in/out. The particles also have a downwards acceleration so they look like they're falling with gravity. Next, we made them spawn more rapid and in a greater distance so it fills the entire room. After, we made them "orbit" which is basically spiral around while doing the rest of the things. Last, we made the particles die out between 4-10 seconds. 

After we got all properties down of the particle, we moved on to the look of the dust particles. First, we made the color gray, like dust, then we made it a circle plane instead of a square plane by using something in the material editor called a Radial Gradient Exponential. We wired that to a multiply block with the Alpha from the Particle Color connected with it, then wired that to the Opacity of the dust particle. This made the particle circular and faded away with transparency in a certain part. Next thing we needed is the dust to fade away to inexistance when the camera gets close to it. First, we would need a Distance_Blend block. Next, we would need two of a thing called a Constant or a Material Expression Constant. We would need to set the Blend Range to 200m and the Start Offset to be -100m. The last thing we did was take the Multiply output from the Opacity and connect that to a new Multiply with our new Distance_Blend and connect that to Opacity.

This was the last thing required for this section, but at the end of the last video, he said to go back and make a new room using everything I learned. He said "he highly recommended it so you're used to" placing meshes and such. So, I went back and created a new room. My room was a theater that went into a door then closed the door behind you. Then, the giant display was playing my previous room video. The camera looked at the tv, moved towards the staircase, went up it, went down to the other end, then down the other staircase, finally it moves to a seat, moves up, then sits in it.


{% include youtubePlayer.html id="2VPiyAL_WKU" %}