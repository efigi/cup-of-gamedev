---
layout: post
title:  "The Importance of Software Accretion"
description:  "Software Accretion is an important concept in Software development! You should apply it to your workflow!"
author: remtaine
categories: ["Programming Principles"]
image: assets/images/pearl.jpg

tags: programming principles createJS Javascript HTML5 software accretion featured
---

I got started on a project earlier. It seemed simple enough; I had the flow of the game already imagined so it was all a matter of just typing it down. I sat down and started coding, checking Google every now and then for the Javascript and CreateJS code needed (I was developing an HTML5 game) for the methods that I had forgotten the syntax of. After some time, I was done. I loaded the HTML page with the JavaScript file linked, and guess what I saw?

A white page.

## What Was Wrong

Of course, I wasn’t that surprised I wasn’t expecting to have written the code perfectly; I expected some bumps here and there. So, I went back to my code and scanned it to see what was wrong. I was hoping it was a mere syntax error or something similar.

It wasn’t. My syntax was correct and all my code seemed to make sense to me. I checked my code several times over and I couldn’t see anything wrong. And yet, it wouldn’t show anything.

## Building Huge Blocks

My problem was that I built it in one huge block and not have not bothered to test it step by step. I built the entire program before even seeing if it could manage to draw anything. Now, to be able to test this properly, I had to comment out large amounts of code just to check if the bare-bones code work. Since the program isn’t that big anyway, I simply scrapped the lot and started anew.

This wouldn’t have happened if I just did software accretion.

## What is Software Accretion?

Software accretion was something mentioned in Code Complete as a metaphor for making a program. It said that one of the best analogies for coding would be the creation of a pearl in an oyster, with it starting small then adding parts little by little. Debugging could be done after adding each tiny feature. This not only makes debugging easier, since it allows to check mainly the code added after the last debug, but also means that debugging would be more organized with adding code parts at a time.

This also forces the programmer to see what is core to the program, seeing what is needed and seeing what is merely an add-on. This is useful especially for those programmers with a deadline, as feature creep (adding more and more features) is a huge cause of delays. Adding it one by one will keep the important parts in the program, so if any parts are missing during launch, it won’t be that bad.

## How I applied it

I forgot about applying this to my coding since it’s been a while since I programmed, but I won’t again. Doing anything else simply isn’t worth the trouble.

Once I rebuilt the code using the principle of Software accretion, things became smoother. I could easily tell when a bug showed up, and I knew immediately which lines of code were at fault. Well, most of the time anyway.

## Software Accretion Everyday

I'm glad that in the end I managed to fix it but next time, I'll build it a bit at a time, checking it every step of the way. That way, I know that something works before I go to the next part. It saves on a lot of development time, and is overall a better way of coding.