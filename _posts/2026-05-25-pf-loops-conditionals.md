---
layout: post
title: "When the Logic Doesn't Loop Right: Wrestling with Conditionals in PF"
date: 2026-05-25
categories:
  - portfolio
  - university
tags:
  - computer engineering
  - programming fundamentals
  - PF
  - university life
  - UET Lahore
---

There is a particular kind of frustration that comes from writing a loop that almost works. Not a loop that crashes immediately and tells you clearly what went wrong, but one that runs, produces output, and looks correct at first glance — until you check the numbers carefully and realize something is subtly off. I spent a significant part of the week following my first PF struggles deep in exactly that kind of frustration, working through loops and conditionals in a way that taught me more about careful thinking than any single lecture could have.

Loops and conditionals are, on the surface, two of the simplest ideas in programming. A conditional lets a program make a decision: do this if a condition is true, do something else otherwise. A loop lets a program repeat an action multiple times without the programmer having to write that action out by hand for every repetition. Described this way, both ideas sound almost too obvious to be worth a whole week of lectures and labs. But the gap between understanding what a loop does in principle and being able to write one correctly under pressure turned out to be much wider than I expected.

My first real encounter with this gap came during a lab exercise that asked us to write a program counting how many numbers in a given range were divisible by a specific value. It seemed straightforward: loop through the range, check divisibility using the modulus operator, increment a counter when the condition was true. I wrote what I believed was a correct solution within a few minutes, ran it, and got an answer that was off by exactly one. That single off-by-one error sent me down a path of careful debugging that taught me more about loop boundaries than any explanation could have. I had set my loop to start from the wrong index, including one extra number that should not have been counted. It was a tiny mistake, almost embarrassingly small once I found it, but it took nearly half an hour of staring at correct-looking code before I noticed it.

This experience introduced me to what I now think of as one of the most important habits in programming: never trusting that code is correct just because it produces an answer. A program can run successfully and still be wrong, and the only way to catch that kind of error is to test deliberately, with specific cases chosen to expose edge conditions rather than just the easy, obvious cases. I started, from that week onward, testing my code with boundary values first — the smallest possible input, the largest possible input, an input of zero — because I had learned the hard way that these boundary cases are exactly where careless mistakes tend to hide.

Conditionals brought their own version of this lesson, particularly once we moved beyond simple if-else statements into nested conditionals and combinations of logical operators. I remember a specific assignment that asked us to classify a triangle based on the lengths of its three sides — equilateral, isosceles, or scalene, while also checking whether the given lengths could even form a valid triangle in the first place. My first attempt checked the triangle type correctly but completely ignored the validity check, happily classifying combinations of side lengths that could never form an actual triangle. Going back and restructuring that logic taught me something about the order in which conditions should be checked — validity first, classification second — that felt almost philosophical in how directly it mapped onto careful reasoning in general, not just programming.

What I found most valuable about this period of the course was how it forced a kind of intellectual honesty that I was not used to. In many of my earlier academic experiences, partial understanding could often be disguised through confident writing or a plausible-sounding explanation. A loop does not accept partial understanding. It either does exactly what you told it to do, or it does something else entirely, and there is no room to talk your way around the difference. I found this unforgiving quality of programming oddly comforting, even in the middle of my frustration, because it meant that genuine understanding was the only path to a working program. There was no shortcut available.

By the end of this week of loops and conditionals, I had developed a working habit that would carry me through the rest of the semester: tracing through code by hand, line by line, on paper, whenever a program behaved unexpectedly. Rather than randomly changing lines of code and hoping the problem would disappear, I forced myself to simulate the program's execution manually, writing down the value of every relevant variable at each step. This was slow, and at first it felt almost like admitting defeat — surely a real programmer should be able to spot the bug just by reading the code. But this slow, methodical tracing caught errors far more reliably than guessing ever did, and it remains, even now, the first thing I reach for whenever something in my code does not behave the way I expect.

Looking back at this week from later in the semester, I can see it as a kind of initiation into the actual discipline of programming, separate from simply learning syntax. Anyone can learn what a for-loop looks like in a particular language within an hour. Learning to think carefully enough that your loops and conditionals do exactly what you intend, every single time, across every case — that takes longer, and it takes the kind of patient, humbling practice that this week gave me in abundance. It is the kind of discipline that [Dr. Bilal Ahmad](https://www.facebook.com/Dr.BilalAhm) consistently reinforced across both courses he taught us this semester, and one I now carry into every technical problem I face.

#ComputerEngineering #ProgrammingFundamentals #PF #UETLahore #LearningJourney #DrBilalAhmad #MLwithDrBilalAhmad
