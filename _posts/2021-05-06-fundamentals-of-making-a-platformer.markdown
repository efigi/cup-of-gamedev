---
layout: post
title:  "Fundamentals of Making a Platformer Game"
description:  "A platformer isn't as simple as making a player and things to jump on! A lot of things are needed to make the game feel right!"
author: remtaine
categories: ["Game Jam"]
image: assets/images/one-arrow-rampage-v1.png

tags: games showoff gamejam postmortem platfomer grapple 2D Godot
---

## Godot Wild Jam

So I made a game called One Arrow Rampage, a fast-paced platformer where you grapple around the area while going on a murder spree! I made it for the [Godot Wild Jam](https://godotwildjam.com/), a jam where people take advantage of the Godot game engine and export to multiple platforms. This was my first jam to do alone, so I had to make do with a lot of things by myself. 

The theme was "Connections", so the first thing that came to my head was grappling hooks for some reason. I was playing around with  possible ideas and I ended up with an arrow/grappling hook that can kill enemies at the same time as zipping towards them. It did pretty well, with a lot of people claiming that it was their favorite in the jam.

The story of the game was:

> You're the finest archer in the kingdom, part of the most elite squad handpicked by the king. One day the king decided you were no longer of any use to him, so he sent the rest of your squad to get rid of you.
>
> With your skills, you survived the assassination attempt. Now you're going to take revenge against your former comrades.
>
> They confiscated your weapons so you only have a bow, some rope, and one arrow, but that's all you need.

## Important Parts

It's my first time doing a platformer, so I learned a lot about proper player movement in this genre. Particularly, there are several key concepts that allow you to move in a better way around the game world. Some are subtle, some are incredibly obvious, but all create a more seamless experience for the player.

Now, take note that not all platformers use these, and some ignore several of these concepts for their own game. Just know that each of those choices are deliberately done, with the game designers having a definite reason as to why they didn't include that particular method when moving. When combined, it allows for a platformer that feels unique and moves in its own special way.

## Air Control

Air control is essentially the act of moving even when in middle of a jump. In real life, when one jumps, it's impossible to change momentum in the mid-air. In the gaming world however, it's possible. In fact, sometimes you can even move to the opposite direction after a jump! This allows the player to fine-tune their movement in between a jump, correcting mid-air so they don't miss a platform or end up hitting an enemy.

When this isn't included, it tends to feel clunky as once the character's feet leaves the air, the player loses control over the character. Ideally, the player never loses control of the character as that tends to ruin the fun. To preserve some degree of skill needed, some platformers would make sure air control isn't as fast as moving on the ground, or it wouldn't allow changing directions in mid-air. Either way, most platformers would allow some degree of control in mid-air.

## Accelerated Running

The most basic way to move a character when programming a game would be to immediately make the player move at a certain speed when pressing the arrow keys or directional pad. When running in platformers however, most games would instead add some acceleration to the character's current speed until it reaches a max speed. 

This effect tends to be subtle as in most platformers, the player would reach maximum running speed a few frames after starting the run. Even so, that several frame difference feels completely different from an immediate max speed move right at the start of the run. Certain games would also make the start-up run slower until it reaches maximum speed, though those games tend to use it to increase difficulty or force the player to never get hit or stop moving.

## Friction

In the same way as accelerated running, it'd be best not to immediately stop the player character once they no longer click the directional keys. Once the player is idle, friction is used to slowly bring the character to a halt. Some platformers even put a skidding animation to show how it's stopping. For precision platformers it'll be only a few frames, but it adds some realistic physics in the game. Be careful not to add a stopping motion that takes too long or covers too much ground however, or else the player will feel like they're walking on ice! 

## Reactive Turning

Reactive turning is related to both accelerated movement in friction, as it refers to how the player changes directon when running or walking. When moving on the ground, most platformers would not make the player immediately change direction when switching direction keys (ie. right to left or left to right arrows). There would be some frames to show the complete shift in momentum. It depends on the kind of platformer as to how fast the shift would be, with more frames being more difficult to control. Adding this sort of turning really helps ground the charactor with more realistic physics.

## Non-Analog Jumping

This sort of concept allows the player more control with regards to the height of the jump. Non-analog jumping is essentially changing the height of the jump depending on the length of the press. Light taps being short jumps while holding the jump button creates the highest jump possible. This allows the player even more control of the jump and let's them jump on platforms easier. It helps create more fluidity in the game as the character can always just jump as much as needed.

## Coyote Time

Coyote Time is named after Wile E Coyote from the Looney Tunes, with his memorable scenes of running over cliffs and only falling when he notices the ground (or rather, lack of it).  In platformer games, coyote refers to how a player could run a few pixels past the edge of a platform without falling, and can consequently jump off as if there was an invisible platform supporting them. Of course, if the player stops moving while mid-air or just spends too long in that area, they will start falling. This allows players to move fast and run off platforms then jump with more leeway.

## Jump Call Tolerance or Buffering

Jump buffering or jump call tolerance refers to when you click the jump button too early, usually when the charcter is still above the ground, but the character jumps on contact with the floor anyway. This adds convenience to the player as they don't need to wait for the precise frame that the player lands on the floor for the jump to work. This is usually done by not only checking if the jump button was just pressed, but also if it was pressed a few frames or milliseconds ago. It really helps add to the fluidity of the moment.

## Weighty Jumping 

Jumping in platformer games aren't super intuitive, and using a normal value for gravity tends to give players that floating feeling. That's why gravity tends to be an important part of making a platformer, as it would dictate the distance between platforms, and how the player can reach the different parts of your game. To add more weighty jumping, make sure to tweak the gravity values, making them a bit bigger.

There was actually a GDC talk about this a while back on Youtube: [Math for Game Programmers: Building a Better Jump](https://www.youtube.com/watch?v=hG9SzQxaCm8). It talks about physics of jumping and how to get rid of the weighty feeling. Essentially, it talks about increasing the gravity as well as making gravity have a greater effect when the the velocity on the Y axis is positive (programming-wise), or in other words falling. If you have the time, I really suggest that you watch it! It's really informative. 

## Too Easy?

I'm sure once people read all these things, some would ask, "but doesn't this make the game too easy?" At first glance it does, as it tends to allow the player to make more mistakes and forgives certain misteps while playing. However, it's these steps that allow a more responsive feeling and makes sure that the player wouldn't have to blame things like their controller, or sudden lag caused by faulty hardware. More importantly, these steps make movement more fluid and allow them to get in the "flow", the zone that you want the players to stay in. Missing a jump by a few pixels or due to clicking a frame too early will annoy the player to no end. By applying these concepts, there will be less moments of "but I clicked it!" and then blaming something else but their skill.

## Conclusion

Even if you've read the concept, realize that fine-tuning them is needed, and is best done through playtesting! Especially when one of your mechanics is a movement-based as a grapple mechanic or other platformer movements. Make sure to always tweak the values to make sure that it creates the best version of your game.

I'll probably make another article in the future on how to implement these concepts from a programming perspective into various game engines. The first one would most probably be on the [Godot Engine](https://godotengine.org/).

You can check out One Arrow Rampage at the <a href="https://remtaine.itch.io/one-arrow-rampage">Itch.io website</a>.

