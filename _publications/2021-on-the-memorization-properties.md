---
header:
  teaser:
    "2021-on-the-memorization-properties.jpg"
title: "On the Memorization Properties of Contrastive Learning"
authors: >
  <b>Ildus Sadrtdinov</b>, 
  <a href="https://nadiinchi.github.io/">Nadezhda Chirkova</a>,
  <a href="https://tipt0p.github.io/">Ekaterina Lobacheva</a>
collection: publications
permalink: /publication/2021-on-the-memorization-properties
date: 2021-07-24
venue: "Workshop on Overparameterization: Pitfalls & Opportunities at ICML"
links: >
  <a href="https://arxiv.org/abs/2107.10143">arXiv</a> /
  <a href="../files/2021-on-the-memorization-properties.bib">bibtex</a>
tldr: >
  We study how different training paradigms (supervised learning, self-supervised
  learning, and training with random labels) learn training examples. We show that
  memorization of self-supervised algorithm (SimCLR) is similar to training with
  random labels.
---

Memorization studies of deep neural networks (DNNs) help to understand what patterns
and how do DNNs learn, and motivate improvements to DNN training approaches.
In this work, we investigate the memorization properties of SimCLR, a widely used
contrastive self-supervised learning approach, and compare them to the memorization
of supervised learning and random labels training. We find that both training objects
and augmentations may have different complexity in the sense of how SimCLR learns them.
Moreover, we show that SimCLR is similar to random labels training in terms of
the distribution of training objects complexity.