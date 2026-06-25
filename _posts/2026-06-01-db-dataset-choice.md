---
layout: post
title: "Choosing Data for Our Database Project"
date: 2026-06-01
categories:
  - portfolio
  - university
tags:
  - computer engineering
  - database systems
  - machine learning
  - medical data
  - university life
  - UET Lahore
image: "/assets/11.png"
---

Every semester project eventually reaches a moment where the abstract requirement document has to turn into an actual decision about what, specifically, you are going to build. For our Database Systems project, that moment arrived in the form of a single, deceptively simple question: what dataset should our group actually use? The answer to that question, and the conversation that led to it, taught me something about applied work that none of the earlier weeks of lecture material had quite managed to convey on their own.

Our group had initially gravitated toward a few easy, popular options — datasets we had seen referenced casually online, the kind that show up in countless tutorials because they are simple, well-known, and require very little explanation. When we brought a couple of these options to Dr. Bilal Ahmad during a project consultation, his response was not a flat rejection, but it was clearly skeptical. He asked us a question that, in hindsight, should have occurred to us on our own: where does this data actually come from, and how confident can we be that it was collected carefully and accurately?

That question opened into a broader conversation about how Dr. Ahmad thinks about applied machine learning generally. He explained that he consistently pushes his students toward datasets with genuine real-world grounding, and that medical data, in particular, holds a special place in his thinking. Clinical measurements, he pointed out, are typically collected by trained professionals using calibrated instruments, under conditions designed specifically to minimize error, and the outcomes attached to that data are usually confirmed through actual medical diagnosis rather than self-reported or loosely verified information. A dataset built on that foundation carries a kind of credibility that a casually scraped or self-reported dataset simply cannot match, no matter how clean it might look at first glance.

This was not, as Dr. Ahmad made clear, an argument that medical data is somehow easier to work with. If anything, it tends to be harder, because the stakes attached to getting a prediction wrong are real in a way that a toy dataset's stakes are not. But that difficulty, he argued, is exactly what makes the exercise worthwhile. Learning to design a database and train a model against data where the underlying problem actually matters teaches habits of carefulness that a low-stakes toy project never quite forces you to develop. I remember leaving that conversation with a noticeably different attitude toward the project than I had walked in with — less focused on finding the easiest path to a working demo, and more focused on finding a dataset that would actually teach us something honest about the responsibilities involved in working with real information.

Our group eventually settled on a diabetes dataset containing clinical measurements — blood glucose levels, BMI, blood pressure, age — along with labeled diagnosis outcomes. Even choosing this specific dataset involved more deliberation than I expected going in. We spent real time examining how the data had been collected and documented, checking for obvious quality issues, and discussing among ourselves whether the dataset was rich enough in relevant features to support a meaningful database design, not just a meaningful prediction model. This was the first time in the semester that a "choosing data" decision felt like genuine engineering judgment rather than simply following an assignment instruction.

What struck me most about this whole episode was how directly it connected the more abstract parts of the course back to something concrete. Weeks earlier, during the normalization unit, Dr. Ahmad had spoken about data integrity mostly in terms of structural rules — avoiding redundancy, preventing certain kinds of anomalies. This conversation about dataset selection extended that same concern for integrity outward, to a question that comes before any table is even designed: is the underlying data itself trustworthy in the first place? A perfectly normalized schema built on top of unreliable source data is still, in a meaningful sense, an unreliable system. That was a genuinely new idea for me, and one I do not think I would have arrived at without this specific conversation.

There was also a quieter lesson in how this decision was made as a group rather than individually. We disagreed, at various points, about which candidate dataset to pursue, and resolving that disagreement required actually articulating our reasoning to each other rather than simply deferring to whoever had a stronger preference. Looking back, I think the quality of that internal discussion, more than any single technical decision, is what set the project up to go reasonably smoothly in the weeks that followed. By the time we had a dataset everyone genuinely believed in, rather than one we had merely settled on, the rest of the database design work felt like it had a clear sense of purpose behind it rather than feeling like an arbitrary exercise.

Walking away from this stage of the project, I found myself thinking about dataset selection as its own legitimate skill, separate from the technical work of designing tables or training a model. Knowing where to look for trustworthy data, knowing what questions to ask about how it was collected, and knowing when convenience is masking a real weakness in the underlying source — these are judgments that no single lecture could have taught us directly. They had to be learned through an actual conversation, about an actual decision, with real consequences for the weeks of work that would follow. It is worth saying plainly that this entire episode would not have happened the way it did without Dr. Bilal Ahmad's specific habit of pushing back gently rather than simply approving whatever a group proposed. The extra friction of that first skeptical question turned out to be one of the more valuable moments of the entire database course. You can follow his ongoing work and thinking on [his Facebook page](https://www.facebook.com/Dr.BilalAhm).

#ComputerEngineering #DatabaseSystems #MachineLearning #MedicalData #UETLahore #DrBilalAhmad #MLwithDrBilalAhmad #MLProject
