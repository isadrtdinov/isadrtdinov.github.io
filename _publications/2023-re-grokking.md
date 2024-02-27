---
header:
  teaser:
    "2023-re-grokking.jpg"
title: >
  [Re] "Towards Understanding Grokking"
authors: >
  <a href="https://scholar.google.com/citations?user=a7Mq82AAAAAJ&hl=en">Alexander Shabalin*</a>,
  <b>Ildus Sadrtdinov*</b>, 
  Evgeniy Shabalin
collection: publications
permalink: /publication/2023-re-grokking
date: 2023-07-20
venue: "ML Reproducibility Challenge 2022"
links: >
  <i>Outstanding Paper Honorable Mention</i> <br>
  <a href="https://openreview.net/pdf?id=Vz9VLcJqKS">pdf</a> /
  <a href="https://openreview.net/forum?id=Vz9VLcJqKS">openreview</a> /
  <a href="https://github.com/isadrtdinov/grokking-reproduction">code</a> /
  <a href="../files/2023-re-grokking.bib">bibtex</a>
tldr: >
  We successfully reproduce results of the paper “Towards Understanding Grokking:
  An Effective Theory of Representation Learning”. We investigate the consistency
  of training phases depending on data and weight initialization and propose smooth
  phase diagrams.
---

In this work, we attempt to reproduce the results of the NeurIPS 2022 paper 
"Towards Understanding Grokking: An Effective Theory of Representation Learning".
This study shows that the training process can happen in four regimes:
memorization, grokking, comprehension and confusion. We first try to reproduce the
results on the toy example described in the paper and then switch to the MNIST dataset.
Additionally, we investigate the consistency of phases depending on data and
weight initialization and propose smooth phase diagrams for better visual perception.

**Methodology &mdash;**
There is no open-source code for the paper. Therefore, we re-implemented all described
experiments by ourselves. We also used the code provided by the authors to validate
training hyperparameters not stated in the paper. As for the computational resources,
we spent around 30 CPU and 125 GPU hours on the NVIDIA V100 GPU.

**Results &mdash;**
We succeeded in reproducing phase diagrams for the toy example. For the MNIST dataset,
we observed a behavior similar to the one from the paper. We used a wider range of
hyperparameters leading us to an extra area with the memorization phase. We also argue
that the original memorization phase is even more delayed grokking. Therefore,
the authors' findings about the MNIST phases are incomplete.

**What was easy &mdash;**
After receiving additional instructions from the authors about the details not
mentioned in the paper, the reproduction of all results was easy because the authors
put significant work into the setup description. Moreover, it was easy to suggest
new experiments, as they followed logically from the previous.

**What was difficult &mdash;**
Generally, it was difficult to reproduce the results because some critical
hyperparameters (the activation function for the toy model and the batch size for MNIST)
were not stated in the paper. Considering MNIST, it took too much time to iterate
over all hyperparameters' values, as grokking requires about 100k training iterations,
which is approximately 30 minutes on the V100 GPU.

**Communication with original authors &mdash;**
We contacted the authors two times and asked for the validation of the setup.
They responded quickly and were very helpful. The authors provided us with the code
for the toy example and the MNIST dataset. We did not execute it for our experiments
but used it for checking the training details and hyperparameters.