---
title: >
  To Stay or Not to Stay in the Pre-train Basin:
  Insights on Ensembling in Transfer Learning
collection: talks
type: "Paper presentation"
permalink: /talks/2023-fall-into-ml
venue: "Fall into ML 2023: Conference on Machine Learning at HSE University"
date: 2023-10-28
location: "Moscow, Russia"
language: "English"
---

[Paper link](https://isadrtdinov.github.io/publication/2023-to-stay-or-not-to-stay) / 
[Presentation recording](https://youtu.be/2-vzNMMMWoI?si=46cb43Rl9bEL3Cih&t=136)

**Abstract:** Transfer learning and ensembling are two popular techniques for improving the performance
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