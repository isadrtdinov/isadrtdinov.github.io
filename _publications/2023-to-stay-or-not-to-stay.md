---
header:
  teaser:
    "2023-to-stay-or-not-to-stay.jpg"
title: >
  To Stay or Not to Stay in the Pre-train Basin:
  Insights on Ensembling in Transfer Learning
authors: >
  <b>Ildus Sadrtdinov*</b>, 
  <a href="https://scholar.google.com/citations?user=4dlh3pkAAAAJ&hl=en">Dmitrii Pozdeev*</a>,
  <a href="https://scholar.google.com/citations?user=7HU0UoUAAAAJ&hl=en">Dmitry Vetrov</a>,
  <a href="https://tipt0p.github.io/">Ekaterina Lobacheva</a>
collection: publications
permalink: /publication/2023-to-stay-or-not-to-stay
date: 2023-12-01
venue: "Neural Information Processing Systems (NeurIPS)"
links: >
  <a href="https://arxiv.org/abs/2303.03374">arXiv</a> /
  <a href="https://openreview.net/forum?id=NNooZoQpP4">openreview</a> /
  <a href="https://neurips.cc/virtual/2023/poster/71864">poster & video</a> /
  <a href="https://x.com/KateLobacheva/status/1734344960579936568">X thread</a> /
  <a href="https://github.com/isadrtdinov/ens-for-transfer">code</a> /
  <a href="../files/2023-on-the-memorization-properties.bib">bibtex</a>
tldr: >
  We study the effectiveness of the exploration of the pre-train basin
  and its close vicinity for ensembling in transfer learning. We show that
  ensembles trained from a single pre-trained checkpoint may be improved by better
  exploring the pre-train basin, while leaving the basin results in degradation
  of the ensemble quality.
---

Transfer learning and ensembling are two popular techniques for improving the performance
and robustness of neural networks. Due to the high cost of pre-training, ensembles of
models fine-tuned from a single pre-trained checkpoint are often used in practice.
Such models end up in the same basin of the loss landscape, which we call
the pre-train basin, and thus have limited diversity. In this work, we show that
ensembles trained from a single pre-trained checkpoint may be improved by better
exploring the pre-train basin, however, leaving the basin results in losing
the benefits of transfer learning and in degradation of the ensemble quality.
Based on the analysis of existing exploration methods, we propose a more effective
modification of the Snapshot Ensembles (SSE) for transfer learning setup, StarSSE,
which results in stronger ensembles and uniform model soups.