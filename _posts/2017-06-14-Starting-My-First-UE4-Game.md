---
layout: post
title: "Starting My First UE4 Game"
date: "2017-06-14T23:55:00-05:00"
projects: [Pinball Game]
tags: [Learning, Courses, Game Design Fundamentals, UE4, Materials, Sound, BSPs]
excerpt: "Today, my work was starting my first game in UE4 a part of the Udemy course I've been taking. The first game is a pinball game."
images: [[woah.png]]
---

Things I learned today:
- Learned how to add emissive properties to materials
- Added texture in material
- Learned how to do Ticks/Impulses
- Line Traces
- Delta Seconds
- Lerps
- Roughness
- Construction Script Usage
- Enums
- Rotator Type Variables
- Sound Cues
- Playing Sound
- Getting Actors of a Class
- Sequences
- ForEachLoops
- Switches
- UI

Today, my work was starting my first game in UE4 a part of the Udemy course I've been taking. The first game is a pinball game. The first thing we did in the beginning of the course was test out the ball. We didn't make a traditional tilted base like a pinball table is, but instead we made the ball have a constant velocity towards the Z Axis of 200. After, we created a stickiness factor that made the ball have some friction so the ball doesn't just fly down but it sort of "falls". Then, we created the base with geometry brushes like last course. This table we created, for now, only had the inside cut out and had a wide barrier on the outsides. We also did line traces to detect when the ball hits the ground.

After the table was done, we got down to the functionality of the table by doing the ball blueprint first. Before, we made a material for a mesh we imported. The material was just shiny and grayish. Next, we applied that material to the mesh. After, we applied the mesh to our BP_Ball. After the ball was done we moved on to the bumper. First, we imported a texture for the bumper, sounds, and the meshes (bumper mechanism and base). Next, we made a material with the texture in it. The texture, when applied on a plane, said, "Hit me for 100 points". We then made two colors, white and blue so we hooked that up to a multiply and lerp making a sort of in between color. We hooked up a "emissiveboost" which just boosted the emissive part of the texture which was the blue texture. Then we hooked everything up to the correct positions. Next, we hooked the bumper parts to do the right things in a blueprint. We also added a thing called a Sound Cue which holds sounds and plays them in any order. We made the Sound Cue play bumper sounds, 5, randomly and modify them slightly in pitch and volume every time it gets played so they don't sound alike. Next, we hooked that up to play the Sound Cue right after impact of the ball. The next thing we did was the flippers. First, we imported the mesh. Next, we made a material that's plastic and made two material instances with a color property on them. We made one white and one yellow. Then, we applied those colors to the mesh like always. Next, we made a flipper blueprint and applied the mesh in there. After, we made a Enumerator with a value of Left Flipper and one more of Right Flipper. Then in the BP_Flipper, we detected whether or not in the editor we set it to a left or right flipper and flip it according to that. Then we did the movement depending on that. After that we did the plunger like the past pieces of the pinball machine and we made a plunger tunnel to for the ball to travel from.

Since we got the functionality working, we made the ball spawn in and respawn by creating a GameMode. We also added inputs for the plunger and the flippers. After that, we created a zone below the the flippers in the "pit" and so when the ball collides with that zone it calls SpawnBall.

After that we added a simple scoring and multiplier system (mostly scoring). The scoring was attached to the GameMode and every time the ball hit one bumper it would +10 points and then have a multiplier, if we have one, but we didn't add one yet. Then we made a UI system where the score prints at the top of the screen.

{% include image.html filename="woah.png" description="Game" %}