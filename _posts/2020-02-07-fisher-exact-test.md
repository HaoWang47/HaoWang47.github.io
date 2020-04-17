---
title: 'Fishy Fisher’s Exact Test'
date: 2020-02-07
permalink: /posts/2020/02/blog-post-5/
tags:
  - STAT
  - Notes
---


Interesting, I never learnt Fisher's exact test when I was undergrad. Or, my mind was out of the classroom when my professor was addressing this test. But in my very first Statistical Inference class when I was sophomore, Dr. Pu (Xiaolong) introduced hypothesis test with the Lady Tasting Tea experiment. I did not know this experiment was firstly mentioned by Sir R.A. Fisher (well, I did not know Fisher back then anyway). I found it the scenario very interesting and started to have a basic idea of what hypothesis testing is. Recently, Dr. Liu mentioned Fisher's Exact Test under the topic of Gene Differential Expression Analysis and talked about the Lady Tasting Tea story.

Before we go to Fisher's Exact Test, I want to describe the Lady Tasting Tea experiment again to refresh my memory. 

## Lady Tasting Tea Experiment

A LADY declares that by tasting a cup of tea made with milk she can discriminate whether the milk or the tea infusion was first added to the cup. We will consider the problem of designing an experiment by means of which this assertion can be tested. … 

Our experiment consists in mixing eight cups of tea, four in one way and four in the other, and presenting them to the subject for judgment in a random order. The subject has been told in advance of what the test will consist, namely that she will be asked to taste eight cups, that these shall be four of each kind, and that they shall be presented to her in a random order, that is in an order not determined arbitrarily by human choice, but by the actual manipulation of the physical apparatus used in games of chance, cards, dice, roulettes, etc., … Her task is to divide the 8 cups into two sets of 4, agreeing, if possible, with the treatments received.

(from The Design of Experiments (London, Oliver and Boyd, 260pp.))

So, there are $C^4_8$ ways to determine the tea infusion in total (distributing the four "milk-first" cups among the 8). If the lady cannot tell the difference, which is our null hypothesis, then the probability that her labeling exactly matches the truth is thus $1/C^4_8=1/70=1.43%$. Now, the question is, how many cups of tea need to be correctly labeled to support lady's declare? It is very likely that she could tell the difference but she miss-labeled one cup (actually two cups since she will have mislabeled a milk-first as tea-first, and vice versa). If she did only mislabel two cups of tea, what is the chance that this randomly happened under null? It is $C^3_4*C^1_4/C^4_8=16/70=22.9%$. Wow, so this (she only mislabeled one pair of cups) actually very likely will happen even if the lady cannot tell the difference. To control the type I error rata (she cannot tell the difference but I accepted her claim), we should reject her claim unless she labeled all cups of tea correctly. In fact, she did. 

## Fisher’s Exact Test
 
Now let's go back to Fisher’s Exact Test. 