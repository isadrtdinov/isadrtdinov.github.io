---
header:
  teaser:
    "2024-where-do-large-lrs.jpg"
title: >
  Where Do Large Learning Rates Lead Us?
authors: >
  <b>Ildus Sadrtdinov*</b>, 
  <a href="https://scholar.google.com/citations?user=BGVWciMAAAAJ&hl=en">Maxim Kodryan*</a>,
  <a href="https://scholar.google.com/citations?user=lvAKVn4AAAAJ&hl=en">Eduard Pokonechny*</a>,
  <a href="https://tipt0p.github.io/">Ekaterina Lobacheva<sup>†</sup></a>,
  <a href="https://scholar.google.com/citations?user=7HU0UoUAAAAJ&hl=en">Dmitry Vetrov<sup>†</sup></a>
collection: publications
permalink: /publication/2024-where-do-large-lrs
date: 2024-12-13
venue: "Neural Information Processing Systems (NeurIPS)"
links: >
  <a href="https://arxiv.org/abs/2410.22113">arXiv</a> /
  <a href="https://openreview.net/forum?id=G5lMFOtFHa">openreview</a> /
  <a href="https://neurips.cc/virtual/2024/poster/95929">poster & video</a> /
  <a href="https://x.com/KateLobacheva/status/1866371463487631859">X thread</a> /
  <a href="https://github.com/isadrtdinov/understanding-large-lrs">code</a> /
  <a href="../files/2024-where-do-large-lrs.bib">bibtex</a>
tldr: >
  We show that only a narrow range of large LRs is beneficial for generalization
  and analyze it from the loss landscape and feature learning perspectives.
---

It is generally accepted that starting neural networks training with large learning rates (LRs)
improves generalization. Following a line of research devoted to understanding this effect,
we conduct an empirical study in a controlled setting focusing on two questions:
1) how large an initial LR is required for obtaining optimal quality, and
2) what are the key differences between models trained with different LRs?
We discover that only a narrow range of initial LRs slightly above the convergence threshold
lead to optimal results after fine-tuning with a small LR or weight averaging. By studying
the local geometry of reached minima, we observe that using LRs from this optimal range allows
for the optimization to locate a basin that only contains high-quality minima.
Additionally, we show that these initial LRs result in a sparse set of learned features,
with a clear focus on those most relevant for the task. In contrast, starting training with too small LRs
leads to unstable minima and attempts to learn all features simultaneously, resulting in poor generalization.
Conversely, using initial LRs that are too large fails to detect a basin with good solutions and
extract meaningful patterns from the data.
