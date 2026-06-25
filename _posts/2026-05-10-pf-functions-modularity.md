---
layout: post
title: "Breaking Problems Into Pieces: What Functions Taught Me About Thinking Clearly"
date: 2026-05-10
categories:
  - portfolio
  - university
tags:
  - computer engineering
  - programming fundamentals
  - PF
  - university life
  - UET Lahore
image: "/assets/2.png"
---

There is a moment in learning to program when a switch quietly flips, and you stop thinking of a program as one long sequence of instructions and start thinking of it as a collection of smaller, well-defined pieces that work together. For me, that moment arrived during the week we spent on functions in Programming Fundamentals, and it changed how I approached every single assignment that came after it, in this course and beyond.

Before this week, my programs tended to be long, unbroken stretches of code, written top to bottom, doing everything in one continuous flow. It worked, in the sense that the programs ran and usually produced the right output, but it worked the way a tangled ball of string works — functional, technically, but uncomfortable to handle and nearly impossible to fix quickly if something went wrong in the middle. Functions, as our instructor introduced them, offered a different way of working entirely: take a self-contained piece of logic, give it a name that describes what it does, define what information it needs as input and what it produces as output, and then simply call it by name whenever that piece of logic is needed, without rewriting it each time.

The first assignment that really tested this idea asked us to write a small program with several related calculations — computing an average, finding a maximum value, and counting how many values exceeded a certain threshold, all from the same set of input numbers. My first instinct, shaped by habits from previous weeks, was to write all of this as one long block of code, calculating everything in sequence. It worked, but rereading it afterward, I genuinely struggled to follow my own logic, even though I had written it only an hour earlier. Restructuring the same program into three separate functions — one for each calculation — made an enormous difference. Each function was short enough to understand at a glance, and the main part of the program became almost like a table of contents, simply calling each function in turn and stating clearly what was happening at each step.

This week also introduced the idea of parameters and return values with a precision I had not expected. A function is not just a labeled block of code; it has a defined contract — these are the inputs it expects, and this is the output it promises to produce. I remember being confused, early on, about the difference between a function that modifies something directly and a function that returns a new value without changing anything outside itself. Working through several small bugs caused by this confusion — expecting a function to have changed a variable when it had only returned a new value that I then failed to store — taught me to read function signatures far more carefully than I had been doing. A function's signature, I came to realize, is really a kind of promise, and breaking that promise, even accidentally, leads directly to bugs.

What I found most valuable about learning functions, though, was not the syntax itself but the way it reshaped how I approached problems before writing any code at all. I started, almost without noticing the shift, to break a new assignment down on paper into a list of smaller sub-problems before writing a single function. What does this program need to do, broken into its smallest meaningful pieces? Which of those pieces are simple enough to be a single function, and which need to be broken down further? This habit of decomposition, more than any specific piece of syntax, felt like the actual lesson this week was trying to teach, with functions simply serving as the vehicle for it.

There was a particular assignment toward the end of this week that made the value of this approach completely clear to me. We were asked to write a program that performed several string operations — checking if a string was a palindrome, counting vowels, and reversing the string — and then combine these operations into a single report about a given input string. Several of my classmates, working without functions, produced long, repetitive programs where similar logic appeared multiple times with slight variations, making any later change a matter of hunting down every repeated instance. My version, broken into small, named functions, let me change a single piece of logic in exactly one place if I needed to fix or improve it. Watching a classmate spend twenty minutes finding and fixing the same bug in three different places in their code, while I fixed mine in a single function, was a small but genuinely persuasive demonstration of why this discipline mattered.

Looking back at this week now, I can see how directly it connected to lessons I would encounter again later in the semester, in an entirely different course. The instinct to break a large, messy problem into small, well-defined pieces — each with clear inputs, clear outputs, and a single responsibility — turned out to be exactly the same instinct that good database design rewards, where a complicated real-world system gets broken into clean, well-defined tables rather than one enormous table trying to hold everything at once. I did not see that connection clearly at the time. It became obvious only weeks later, once the database project was well underway, and I found myself thinking about table design with the exact same mental habits this week of functions had quietly built in me.

It is a strange thing, in hindsight, to realize that two courses taught by [Dr. Bilal Ahmad](https://www.linkedin.com/in/drbilalphd/), on the surface covering completely different material, were quietly reinforcing the same underlying discipline from two different directions. Programming Fundamentals taught me to decompose a process into small, named steps. Database Systems, running in parallel, would soon teach me to decompose a structure into small, well-defined pieces. Neither course pointed out this parallel explicitly. It only became visible to me by living through both at once, across the same stretch of the same semester.

#ComputerEngineering #ProgrammingFundamentals #PF #UETLahore #LearningJourney #DrBilalAhmad #MLwithDrBilalAhmad
