---
layout: post
title: "Training and Evaluating Our Diabetes Predictor"
date: 2026-06-02
categories:
  - portfolio
  - university
tags:
  - computer engineering
  - database systems
  - machine learning
  - python
  - university life
  - UET Lahore
image: "/assets/12.png"
---

With our database schema designed, normalized, and populated with real clinical data, our Database Systems project entered the stage I had been most curious about since the very beginning: actually training a model to make predictions from that data. This part of the project sat slightly outside the core syllabus of the course itself, but Dr. Bilal Ahmad had structured the project specifically to push us into this territory, and the week we spent on it taught me as much about discipline and patience as it did about machine learning itself.

Before any model could be trained, the data pulled from our database needed to be prepared, and this preprocessing stage turned out to be far more involved than I had anticipated. Clinical measurements like blood glucose levels, BMI, and blood pressure existed on very different numerical scales, and we learned that many learning algorithms perform poorly, or at least inconsistently, when input features differ this dramatically in magnitude. Scaling the numerical features to a comparable range, encoding categorical values into a form the model could actually use, and splitting the dataset into separate training and testing portions were each, individually, small steps. Combined, they took up a surprising amount of our time, mostly because we kept discovering small inconsistencies in the data that needed to be resolved by hand — a missing value here, an oddly formatted entry there — that no amount of advance planning had fully anticipated.

Training the model itself, once the data was properly prepared, felt almost anticlimactic in comparison to the preprocessing work that preceded it. A few lines of code, calling a library function with our prepared training data, and within a relatively short time we had a trained model sitting in front of us. What was not anticlimactic at all was the moment immediately after, when we had to decide whether that trained model was actually any good. This is where evaluation metrics like accuracy, precision, and recall stopped being abstract terms from a slide and became something we genuinely had to reason about ourselves.

We looked first at accuracy — the proportion of predictions the model got right overall — and it looked reasonably strong at first glance. But Dr. Ahmad, during a brief project check-in, pushed us to look past that single number, asking specifically about precision and recall, and what those metrics meant in the context of a medical prediction task. That question reframed how I understood the model's performance entirely. A model that misses a genuine positive diabetes case is making a very different kind of mistake than a model that occasionally flags a healthy patient unnecessarily, and a single overall accuracy figure blurs that distinction completely. Calculating recall specifically, and seeing how it differed from our overall accuracy figure, was the moment this project stopped feeling like a coding exercise and started feeling like a genuine exercise in responsible judgment.

This conversation pushed our group to examine our model's confusion matrix in detail, breaking down exactly which kinds of errors it was making and how often. We discussed, among ourselves, what an acceptable balance between precision and recall should look like for a task like this, recognizing that the "right" answer depends heavily on the real-world consequences of each kind of error, not purely on which number happens to look more impressive in a results table. I do not think any of us arrived at a fully confident final answer to that question, but the act of seriously asking it, rather than simply reporting whichever metric looked best, felt like real progress in how we were thinking about the project.

Connecting this evaluation work back to the database side of the project added another layer of understanding. The quality of our model's predictions depended directly on the quality of the data we had stored and retrieved, which depended, in turn, on the care we had put into designing and normalizing our schema weeks earlier. A poorly designed database that introduced subtle data quality problems would have shown up here, in the model's performance, even though the immediate cause would have looked, on the surface, like a modeling problem rather than a database problem. Seeing that connection made concrete, rather than just stated in lecture, was one of the more valuable realizations of this entire stage of the project.

By the end of this week, we had a model that performed reasonably well, evaluated honestly rather than optimistically, and a much clearer sense of what "reasonably well" should even mean for a task with real medical stakes attached to it. Watching the prediction pipeline run end to end — from a row of patient data, through our database, into the trained model, and out as a clear prediction — gave me a genuine sense of how the different pieces of this semester's coursework had quietly come together into something larger than any single course had taught on its own. Database design and careful programming discipline, both built up over weeks of separate practice in two different courses taught by [Dr. Bilal Ahmad](https://www.linkedin.com/in/drbilalphd/), converged here, in a project that neither subject could have produced fully on its own.

There was one more lesson from this week that took me a little longer to fully appreciate. We had been so focused, throughout the preprocessing and training stages, on getting the technical pipeline to run correctly that the evaluation conversation with Dr. Ahmad came almost as a surprise, even though it should not have. It is easy, once code finally runs without errors, to treat that as the finish line. This week taught me that running correctly and being correct are two entirely different milestones, and that the second one requires a willingness to interrogate your own results rather than simply being relieved that they exist at all. That distinction, more than any specific metric we calculated, is the thing I expect to carry forward from this stage of the project into whatever data-driven work comes next in my studies.

#ComputerEngineering #DatabaseSystems #MachineLearning #Python #UETLahore #DrBilalAhmad #MLwithDrBilalAhmad #MLProject
