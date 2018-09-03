---
layout: post
title: "Beginning to Make Our Own Game"
date: "2017-06-24T16:11:58+05:30"
projects: [Horde Refined Game]
tags: [Horde Refined Game, Learning, Game Design Fundamentals, UE4, Cameras, Getting Stuck, Dynasty Warriors]
excerpt: "Today, we began going through the list of items we're, Adam and I, going to add to refine our horde style game."
---

Today, we began going through the list of items we're, Adam and I, going to add to refine our horde style game. We started doing the first item, implementing a over the shoulder kind of view like in Dynasty Warriors. We didn't know it would be so hard to implement a simple change of the camera, but my instructor from my Udemy course made the camera system super complicated and it would break since the camera doesn't do anything besides follow the player. But, the player rotates and looks with the mouse, so if we made it behind them slightly instead of top down, the character wouldn't be able to rotate easily or be jittery. So we had to remove all the code and start from scratch after a couple hours of fiddling with the camera, spring arm, and the settings to see what exactly everything did. After hours of fiddling, we figured out how to fix it. We went to the default third person project and took the camera settings and everything else and put it in our blueprint for the character. 

This solved our problem kind of, but it still needed bounds to be set so we could rotate slightly above the character and lock at a certain point. And, when you click it gets rid of the camera moving, the game thinks it wants focus on the UI and the hitting. So, we made it so the game should focus on the game every so often so it detects if you're wanting to move the camera. And that worked. You wouldn't think that it would be that hard to fix a camera, but the way we worked the movement and camera was overly complicated. We spent a day doing that.