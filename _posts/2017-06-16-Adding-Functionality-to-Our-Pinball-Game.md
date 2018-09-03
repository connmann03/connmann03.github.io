---
layout: post
title: "Adding Functionality to Our Pinball Game"
date: "2017-06-16T23:55:00-05:00"
projects: [Pinball Game]
tags: [Learning, Courses, Game Design Fundamentals, UE4, Events, Materials, Programming, Timelines]
excerpt: "Things I learned today: Event Dispatchers, Child Actors in the world, Playing attached sounds, Physics(kinda)"
---

Things I learned today:
- Event Dispatchers
- Child Actors in the world
- Playing attached sounds
- Physics(kinda) 

Today's work was fairly short, but I learned a few things. I continued where I left off and that's at working with splines. I finished splines and I created a thing called a Child Actor. These actors are the same thing as regular actors but are a part of a "Parent" actor. And the Child is a part of the Parent. Think it of a folder on your computer; /Documents/Folder/meme.png. In this example, meme.png is apart of /Folder/ in the /Documents/ folder. So all of /Folder/ is a child to /Documents/ as it is a parent. 

After all of the Child Actor "non-sense", we added things called event dispatchers. Event dispatchers basically tell the blueprint to run lines of blueprint nodes/blocks in this event dispatcher. And that event dispatcher can be hooked up to anything in that blueprint and you can add events to it when calling it. That's exactly what we did.

The next thing we did, was make the slingshots. The slingshots, if you don't know, are the triangular bumper-like things above the (bottom) flippers that have a rubber band around to sling the ball across the table. So, we morphed the band by attaching a thing in the material to the material on the band only. This would be triggered in the blueprint for the slingshot through a dynamic material instance and a timeline of 3 points that look like a triangle. 

After the slingshot was finished, I changed the table and the ball physics since it is unrealistic. I tilted the table, added an invisible plane on top of the table, removed the downwards force on the ball since it broke, and weighed the ball.