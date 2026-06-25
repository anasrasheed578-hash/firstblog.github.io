---
layout: post
title: "Standing in Front of the Panel: Presenting the Diabetes Prediction System at the Database Exhibition"
date: 2026-06-10
categories:
  - portfolio
  - university
tags:
  - computer engineering
  - database systems
  - machine learning
  - exhibition
  - UET Lahore
image: "/assets/14.png"
---

Building the diabetes prediction system was one kind of challenge. Standing in front of a room and explaining it, live, to people who had not spent the last several weeks inside our codebase, turned out to be a completely different one. The exhibition on June 10th was where my group and I had to take everything we had built — the normalized database, the SQL pipeline, the trained model, the web interface — and translate it into something a stranger walking up to our table could understand in a few minutes.

We had agreed beforehand on roughly who would speak to which part of the system, but exhibitions rarely stay inside the lines you drew for them in advance. People did not ask questions in the order we had planned for, and more than once someone wanted to go deeper into one part of the system right as we were trying to move on to the next. I found myself explaining the database schema to one visitor while a groupmate ran the live prediction demo a few feet away for someone else entirely, and we adjusted on the fly to whoever was standing in front of us rather than running through a fixed script from start to finish.

The live demo was the part I had been most nervous about beforehand, and it ended up being a genuine mix of good moments and rough ones. When it worked, it worked well: someone would suggest a set of clinical values, we would enter them into the form, and watch the prediction come back almost instantly, with the audience visibly tracking the number on screen change in response. Those moments justified all the time we had spent making sure the pipeline actually connected end to end rather than just running in isolated pieces during development. But the demo was not flawless. At one point, an input value at the edge of what the model had been trained on produced a result that took a visitor by surprise, and we had to pause and actually explain, honestly, what was happening underneath — that the model's predictions are only as reliable as the range of data it learned from, and that values far outside that range deserve to be treated with more caution rather than blind trust in whatever number the screen shows. It was not the smoothest moment of the day, but in hindsight it forced us to explain the system's limitations clearly instead of letting people walk away thinking it was infallible, which is arguably a more honest outcome than a presentation where nothing ever gets questioned.

Handling people's doubts directly was, in fact, one of the more demanding parts of the whole afternoon. A few visitors asked, reasonably, why anyone should trust a student project's prediction over an actual medical test, and we had to be clear and a little humble in our answer: this was never built to replace a diagnosis, it was built to demonstrate that the underlying pipeline, from raw clinical data through a normalized database through a trained model to a usable interface, could be constructed correctly by us, end to end. Separating the technical achievement of the project from any implied medical authority of its output was a distinction we had to make explicitly, out loud, more than once during the day, and saying it clearly each time actually sharpened how we understood our own project's scope.

Other questions were more technical and, honestly, more fun to answer. A few visitors with some programming background wanted to know why we had bothered with full normalization instead of just dumping everything into one wide table, and explaining the reasoning out loud, rather than just having internalized it silently while building the schema weeks earlier, made me realize how much more solid my own understanding of normalization had become since the actual database design phase. Other questions probed the machine learning side specifically, asking what would happen if the dataset were biased in some way, or imbalanced between diabetic and non-diabetic cases, and fielding those questions live meant drawing on the same evaluation-metric discussions we had had internally as a group during development, except now defending those choices to someone who had every right to be skeptical of them.

Dr. Bilal Ahmad, evaluating the exhibition, asked us a few pointed questions of his own, mostly steering us toward justifying specific design decisions rather than just describing what the system did. Being asked to defend a choice on the spot, in front of an audience, is a noticeably different experience than discussing the same choice privately within your own group, where everyone already shares the same assumptions and context. It meant articulating, clearly and on the spot, why we had made certain decisions the way we had, rather than simply asserting that the decisions had been made.

By the end of the day, what stayed with me most was not any single technical detail of the system, but the experience of communicating it under real conditions, to real people, with real uncertainty about what they would ask next. Writing code and presenting that code to a skeptical audience are genuinely different skills, and the exhibition was the first time this year I had to exercise both of them back to back, in public, with no opportunity to quietly fix something off-screen before anyone noticed. That kind of pressure is uncomfortable in the moment, but I think it taught me something that no amount of solitary coding practice could have: that a project is not really finished until you can explain it, defend it, and acknowledge its limits honestly, all while someone you have never met is standing in front of you waiting for an answer.

#ComputerEngineering #DatabaseSystems #MachineLearning #Exhibition #UETLahore
