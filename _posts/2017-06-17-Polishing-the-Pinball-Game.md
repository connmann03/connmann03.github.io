---
layout: post
title: "Polishing the Pinball Game"
date: "2017-06-17T16:11:58+05:30"
projects: [Pinball Game]
tags: [Learning, Courses, Game Design Fundamentals, UE4, Physics, Vector Transforms, Sound, Materials]
excerpt: "Today's work was adding the last piece of functionality to our game."
images: [[spinner.jpg]]
---

Things I learned today:
- Physics Constraints
- Adding sounds attached to blueprints and modifying the pitch in the blueprint
- Forced Direction Volumes
- Vinterp To
- Clamp
- Getting World Transform
- Inverse Transform Direction
- Camera Rotation
- Tilting Camera/World through a blueprint
- Swizzle (swaps X & Y)

Today's work was adding the last piece of functionality to our game. We added a spinner blueprint with 5 meshes attached to it. One the left bracket, another the right blueprint, one the cylinder beside spinner, another the top bracket, and the spinner tile.

Next, we added a thing called a Physics Constraint. This constraint is a thing that basically welds two objects together and make on the thing that will have collision with anything. All we did was change the angle of the movement to 90 degrees and flipped it so it moves upwards and closes.

{% include image.html filename="spinner.jpg" description="Spinner" %}

Next, we added a thing called a Force Direction Volume. This special volume is a blueprint, but it basically slightly interrupts the movement of any object you select and pushes it into the direction of local X which is the arrow component attached to it. We used a thing called Get World Transform where it gets the world transform of the arrow then we did Inverse Transform Direction. Then, did Vinterp To which reaches the arrow from it's current position and tries to smooth it out and edit it. Then repeated.

We then added a tilting the table function like in actual pinball. It limits it to 3 tilts per game. It rotates the camera like the world is rotating when you tilt the table. 

After all of this functionality adding, we started polishing the game. We added a material with a wood table texture to the base. In that material we did a thing called Swizzle. This thing basically swaps x and y values of a texture so it looks like it doesn't repeat so often and looks natural. Then, we multiplied it by .1 and applied to a color and made it have reddish blackish scratches. Like an old wood table.

{% include youtubePlayer.html id="ZWj0v_fkt8M" %}