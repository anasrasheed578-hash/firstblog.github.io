---
layout: post
title: "Building a Walmart Store Performance Model for the Programming Fundamentals Exhibition"
date: 2026-05-16
categories:
  - portfolio
  - university
tags:
  - computer engineering
  - programming fundamentals
  - PF
  - data science
  - python
  - UET Lahore
---

The first-semester exhibition was the point where Programming Fundamentals stopped being something we practiced in isolated exercises and turned into something we had to actually deliver as a group. My team decided early on that we wanted a project with a real business angle rather than a purely academic toy problem, and we settled on something that felt both ambitious and genuinely useful: building a small model around Walmart store data to figure out which of roughly forty stores were actually making money, which ones were barely breaking even, and which ones were quietly losing it. Looking back, the gap between deciding on that idea in a planning meeting and actually getting a working notebook in front of the exhibition panel was a lot bigger than any of us expected going in.

We started, as most data-driven projects seem to, with the unglamorous part: getting the dataset into a shape we could actually work with. The raw data came in with sales figures spread across stores and time periods, and before any analysis could happen, it had to be loaded, checked for missing or inconsistent entries, and organized so that each store's numbers could be compared fairly against every other store's. We leaned on pandas for almost all of this groundwork, since it gave us a clean way to load the data into a structure we could filter, group, and aggregate without writing manual loops for every operation. NumPy sat underneath a lot of the heavier numerical work, particularly once we moved from simply displaying numbers to actually computing summary statistics across all forty-odd stores at once.

My own role in the group ended up centering on the comparison logic itself, which in hindsight was the part of the project that taught me the most. It is one thing to load a dataset and print it out; it is a different thing entirely to write the logic that decides, in a defensible and consistent way, which store counts as high-performing, which counts as marginal, and which counts as a loss. We could not simply sort stores by raw sales totals and call it a day, because a store with high revenue and disproportionately high costs is not actually the strongest performer, even if its top-line number looks the most impressive on a chart. Writing the comparison logic meant deciding on the right basis for comparison first, and only then writing the code to apply that basis consistently across every store in the dataset, rather than eyeballing a few standout rows and assuming the rest would follow the same pattern.

This is where the habits from earlier in the semester paid off in ways I had not fully expected. The same discipline that arrays had forced on me, double-checking loop boundaries, not trusting a value until every relevant element had actually been processed, turned out to matter just as much when the "array" in question was a column of forty store records instead of a list of test scores. I caught myself, more than once, wanting to flag a store as a clear loss based on an early glance at its numbers, before the full aggregation across that store's records had actually finished running. It was the same underlying bug pattern as the average-and-count mistake from the arrays assignment, just wearing a different costume: judging a result before the computation behind it was actually complete.

Once the comparison logic was in place, the next major piece was making the results legible to someone who had not been staring at the dataset for weeks, which is where data visualization came in. We used Matplotlib for the core charts and Seaborn on top of it for anything where we wanted cleaner default styling without hand-tuning every visual element ourselves. Bar charts ended up doing most of the heavy lifting, since ranking forty stores by income, and grouping them visually into clear high-performing, marginal, and loss-making bands, communicated the finding far faster than a table of forty rows ever could. We also put together a comparative view that let a viewer see, at a glance, roughly how many stores fell into each performance category, rather than forcing them to scan individual bars one at a time.

Working in a group on this added its own layer of complexity that a solo assignment never would have. Dividing the work meant agreeing early on what format the cleaned data needed to be in by the time it reached the comparison stage, since a mismatch there would have meant redoing work under exhibition deadline pressure. We talked through, more than once, what counted as a fair definition of "beneficial" versus "loss" for a store, because that definition was not handed to us, it was something we had to decide on and defend if asked. That discussion alone felt closer to the kind of judgment call that shows up in real analytical work than anything a single-variable exercise earlier in the semester had prepared us for.

By the time we stood in front of the exhibition panel, the project had stopped feeling like a class assignment and started feeling like something we had actually built and could explain, store by store, decision by decision. Presenting it meant being able to answer, on the spot, why a particular store had been classified the way it had, and that kind of accountability is, I think, the real value of an exhibition project: it tests not just whether the code runs, but whether you actually understand what it is doing and why. The comparison logic I had written was no longer just my contribution to a notebook; it was something I had to stand behind out loud.

Looking back at the semester as a whole, the array unit from earlier in the term and this exhibition project felt like two ends of the same thread. One taught me to be careful with a list of numbers small enough to trace by hand. The other forced me to apply that same care at a scale where tracing by hand was no longer an option, and where the only way to trust the result was to trust the logic that produced it. That is, I think, the actual point of a first-semester exhibition: not to produce a polished product, but to find out whether the habits built in small exercises actually hold up once the dataset, the team, and the stakes all get bigger at once.

#ComputerEngineering #ProgrammingFundamentals #PF #DataScience #Python #UETLahore
