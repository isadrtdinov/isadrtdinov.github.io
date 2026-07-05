---
header:
  teaser:
    "2026-can-stationary-distributions.jpg"
title: >
  Can Stationary Distributions of Scale-Invariant Neural Networks Be Described by the Thermodynamics of an Ideal Gas?
authors: >
  <b>Ildus Sadrtdinov</b>, 
  <a href="https://tipt0p.github.io/">Ekaterina Lobacheva</a>,
  <a href="https://scholar.google.com/citations?user=QuC0UyEAAAAJ&hl=en">Ivan Klimov</a>,
  <a href="https://scholar.google.com/citations?hl=en&user=t_PLQakAAAAJ">Mikhail Burtsev</a>,
  <a href="https://scholar.google.com/citations?user=MGcJlikAAAAJ&hl=en">Mikhail Katsnelson</a>,
  <a href="https://scholar.google.com/citations?user=7HU0UoUAAAAJ&hl=en">Dmitry Vetrov</a>
collection: publications
permalink: /publication/2026-can-stationary-distributions
date: 2026-08-15
venue: "International Joint Conference on Artificial Intelligence (IJCAI)"
links: >
  <a href="https://arxiv.org/abs/2511.07308">arXiv</a> /
  <a href="https://github.com/isadrtdinov/neural-nets-ideal-gas">code</a> /
  <a href="../files/2026-can-stationary-distributions.bib">bibtex</a>
tldr: >
  We show that the stationary distributions of scale-invariant networks can be expressed by an ideal gas law. In this interpretation, weight decay acts as pressure, and half of the squared parameter norm acts as volume. 
---

Understanding the training dynamics of deep neural networks remains a major open problem, with physics-inspired approaches offering promising insights. 
Building on this perspective, we develop a thermodynamic framework to describe the stationary distributions of stochastic gradient descent (SGD) with weight decay for scale-invariant neural networks, a setting that both reflects practical architectures with normalization layers and permits theoretical analysis. 
We establish analogies between training hyperparameters (e.g., learning rate, weight decay) and thermodynamic variables such as temperature, pressure, and volume. 
Starting with a simplified isotropic noise model, we uncover a close correspondence between SGD dynamics and ideal gas behavior, validated through theory and simulation. 
Extending to training of neural networks, we show that key predictions of the framework, including the behavior of stationary entropy, align closely with experimental observations. 
This framework provides a principled foundation for interpreting training dynamics and may guide future work on hyperparameter tuning and the design of learning rate schedulers.
