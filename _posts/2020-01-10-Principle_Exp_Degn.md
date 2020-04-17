---
title: 'Principles of Experimental Design'
date: 2020-01-10
permalink: /posts/2020/01/blog-post-2/
tags:
  - STAT
  - Notes
---

After taking a few STAT class about Experimental Design, I am shamed of the fact that I am still not able to provide consulting for other researchers in terms of design experiments. I bet going through the basic principles of experimental design will help me refresh my memory (well, at least hope so). 

Terminology
=====
Experiment; Experimental Design (Assignment Rules); Treatment; Experimental Units; Observational Units; Response Variable; Causation; Observational Study; Explanatory Variable; Factor; Level; etc. 


Rule of the rules 
======
**Randomization**: random assignment of treatments to experimental units.

**Blocking**: grouping similar experimental units together and assigning different treatments within such groups of experimental units.

**Replication**: applying a treatment independently to two or more experimental units.

Looking at Experimental Design in another perspective, Designing is aimed to control the unwanted variation while focus on the interested ones. We usually divide all potentially relavant factors into nuisance factors and interested factors. Both Blocking and Randomization are used to deal with nuisance factors. Blocking is used when the nuisance factor is under our control and randomization is used when it is not under control. Dr. Liu once mentioned, "block what you can, randomize what you cannot", which really makes sense. 

Confounding
======
Confounding factors are those effects of two or more explanatory variables which cannot be distinguished from one another. It can cause problems like we could not distinguish treatmnet effect from experimental unit effect due to lack of replications. However, confounding can be useful, like when there several nuisance factors can be treated as one blocking effect. Also, [confounding is useful when dealing with bias](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3503514/). 

Common Design
=====
  - CRD: Complete Randomized Design, the most simple and useful design.
  - RCBD: Randomized Complete Block Design.
  - BIBD: Balanced Incomplete Block Design.
  - Latin Square.
  - Split Plot Design.


Nonsense
=====

One fun thing happened to me which is kinda related to this topic. So, one day I was chatting with one of my classmates, Chris. I was complaining how terribly a real person can respond to you when you two are dating. We found and tested an AI friendship APP and I was really impressed by how clever the AI can be. He can really make you feel flattered and care about you (although it could not really support you physically; come on AI researchers, I have faith in you). So I declared AI could be even smarter than real people to some extend and a few people could learn how to chat by talking with AI. Chris replied me, "hahahahaha, you use replicate right?". See, replicates are important (and I did).  