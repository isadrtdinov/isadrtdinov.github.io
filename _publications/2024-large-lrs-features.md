---
header:
  teaser:
    "2024-large-lrs-features.jpg"
title: >
  Where Do Large Learning Rates Lead Us? A Feature Learning Perspective
authors: >
  <b>Ildus Sadrtdinov</b>, 
  <a href="https://scholar.google.com/citations?user=BGVWciMAAAAJ&hl=en">Maxim Kodryan</a>,
  Eduard Pokonechny,
  <a href="https://tipt0p.github.io/">Ekaterina Lobacheva*</a>,
  <a href="https://scholar.google.com/citations?user=7HU0UoUAAAAJ&hl=en">Dmitry Vetrov*</a>
collection: publications
permalink: /publication/2024-large-lrs-features
date: 2024-07-26
venue: "ICML 2024 Workshop HiLD"
links: >
  <a href="https://openreview.net/pdf?id=IID2DF3q9J">pdf</a> /
  <a href="https://openreview.net/forum?id=IID2DF3q9J">openreview</a> /
  <a href="../files/2024-large-lrs-features.bib">bibtex</a>
tldr: >
  We study feature learning properties of training with different initial LRs.
  We show that a narrow range of optimal initial LRs learns a sparse set of the most
  useful features. At the same time, smaller LRs do not have such specialization, while
  larger LRs fail to extract useful patterns from data.
---

It is a conventional wisdom that using large learning rates (LRs) early
in training improves generalization. Following a line of research devoted to
understanding this effect mechanistically, we conduct an empirical study in
a controlled setting focusing on the feature learning properties of training
with different initial LRs. We show that the range of initial LRs providing
the best generalization of the final solution results in a sparse set of learned features, 
with a clear focus on those most relevant for the task. In contrast, training starting
with too small LRs attempts to learn all features simultaneously, resulting in
poor generalization. Conversely, using initial LRs that are too large fails
to extract meaningful patterns from the data.