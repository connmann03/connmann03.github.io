---
layout: post
title: "Unreal Engine 4: How to Develop Your First Two Games"
date: "2017-06-11T23:55:00-05:00"
projects: [Apartment ArchViz Scene]
tags: [Learning, Courses, Game Design Fundamentals, UE4, Brushes, BSPs, Geometry Editor, Lighting, Post-Processing, Photo Realistic Architectural Rendering]
excerpt: "Today, I started a course from Udemy on developing my first two games in Unreal Engine 4"
images: [[output_720.gif]]
---

Today, I started a course from Udemy on developing my first two games in Unreal Engine 4 ([Udemy Unreal Engine 4: How to Develop Your First Two Games](https://www.udemy.com/unreale4/)). The first part of the course is learning how to do lighting and post processing effects in UE4. We started out placing geometry volumes or "brushes". After placing them, I learned that you can combine multiple brushes together to make one shape. There is an entire geometry editor in UE4 and I didn't know that. In that separate editor "mode" you can make the brushes extrude out into another separate shape. You can also edit the individual vertices and move them how you want. They blend together and are additive. Then, we changed a sphere inside this wall I created with square brushes to be subtractive so it carved out a circular hole in the wall. This part of the course was really interesting since I didn't know anything about this until now.

After we tested the geometry, we started creating the outline of the room. We made a square room using the top down view in UE4 to make it precise. We then downsized it to one corner since it was too big for what we were going to do. We then started adding lighting since a house needs lighting right? But, anyways we added a sliding door to one side of the room. It was in the wall so we had to make another square brush the size of the doors' window/opening. We had to then move the door into the wall and the brush with it. Then, we changed the brush into a subtractive brush to see if it worked. It did indeed work so we got a sliding door. I continued to decorate the room and then we started post processing effects. But, I checked the clock and it was 12:32 a.m.

{% include image.html filename="output_720.gif" description="Woah" %}

{% include youtubePlayer.html id="wEx1Tpoi0iQ" %}