---
layout: post
title: "Multiplayer And Horrible Bugs"
date: "2018-07-13"
projects: [Mowing Game]
tags: [Mowing Game, UE4, Multiplayer, Bugs, Programming, Wondering In The Woods]
excerpt: "Today was awful but was fun for a bit."
---

Today was awful but was fun for a bit. Today is the day I added multiplayer functionality to the game. I first looked into it a bit but I was still going into it blindly. By that I mean I've never done anything relating to making it work to the slightest bit.

I first started off getting it to be able to have the right grass, fence, tree, and arrow placements. Which wasn't too hard because inside each blueprint, you can make it "replicate" to each client. It's magical.

This next part was a struggle, to correctly replicate a variable from the player to the server to relay it to the other players. Like a player color showing up for other players. It was horrible figuring it out and it was just like looking random things up, trying them out, finding new information about what to do and what works, and then toying around for a little bit to magically get it to work. This was horrible. But in the end we got player color relaying over to other players by making the variable Replicate Notify (RepNotify) which basically I guess notifies the server to change this value and it just works magically. Then I added a death timer so you respawn after 10 seconds. And it displays in the world so other players can see, but we are struggling with the RepNotify to notify a timer handle.