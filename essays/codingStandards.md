---
layout: essay
type: essay
title: "ESLint: Your Overly Anxious Coding Buddy"
# All dates must be YYYY-MM-DD format!
date: 2023-02-07
published: true
labels:
  - Javascript
---

You know those times when you're just about to do a chore, like the dishes for example, and just as you're reaching for the sponge your parent says, "Don't forget to do the dishes!" And in an instant, any will or desire to even touch those dishes is sapped from your soul. A similar experience came from coding with ESLint for the first time. Three lines of code in and it starts barraging you with warnings in red: "Hey this variable is unused, you can't do that >:(," or "Woahh you can't not leave an empty line at the end of your code," or "Did you just use two indents instead of one?? Preposterous." And this whole time I'm thinking, "calm down I'll get there in a second!" 

This tool for coding standards can be a bit dramatic and nags about  things that are seemingly trivial. So what if I use two indents in my next line of code or what if I leave a variable unused? What if I just want my other variable to have a friend? In reality, while these standards are mildly tedious, they are very important in keeping code neat and warding off minor mistakes that could cause trouble later on. When I look back at the code that's been ESLint-approved, everything is neat and highly readable. Omitting unused variables or functions removes any unnecessary distractions and clutter that take away from the important stuff. Additionally, it gives warnings for small issues that might cause issues later on. For example, in the ziplist WOD, I originally created the array that would store the combined arrays as a let variable. ESLint gave a warning that suggested it be changed to const. For ziplist, I wouldn't ever want to reassign that array so it'd would be better to make it a const to prevent myself from accidentally changing it later on. Little catches like this would be especially helpful in actual projects where there are hundreds of lines of code and several different files. Imagine accidentally reassigning a variable from line 2 of file 1 in line 500 of file 9. What a nightmare it'd be to have to try and fix. Coding standards flag minor issues like this, which can help prevent a massive headache in the future.

<img width="200px" 
    src="../img/ok.jpeg">
