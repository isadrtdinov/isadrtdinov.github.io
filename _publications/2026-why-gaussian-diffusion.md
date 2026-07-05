---
header:
  teaser:
    "2026-why-gaussian-diffusion.jpg"
title: >
  Why Gaussian Diffusion Models Fail on Discrete Data and How to Prevent It?
authors: >
  <a href="https://ashaba1in.github.io/">Alexander Shabalin</a>,
  <a href="https://scholar.google.com/citations?hl=en&user=E3XQ25QAAAAJ">Simon Elistratov</a>,
  <a href="https://scholar.google.com/citations?user=FtnaZfsAAAAJ&hl=en">Viacheslav Meshchaninov</a>,
  <b>Ildus Sadrtdinov<sup>†</sup></b>, 
  <a href="https://scholar.google.com/citations?user=7HU0UoUAAAAJ&hl=en">Dmitry Vetrov<sup>†</sup></a>
collection: publications
permalink: /publication/2026-why-gaussian-diffusion
date: 2026-04-02
venue: "arXiv preprint"
links: >
  <a href="https://arxiv.org/abs/2604.02028">arXiv</a> /
  <a href="https://x.com/a__shabalin/status/2062086123405365658">X thread</a> /
  <a href="../files/2026-why-gaussian-diffusion.bib">bibtex</a>
tldr: >
  We explain why Gaussian diffusion models with the DDPM solver perform poorly on discrete domains, and analyze heuristics (self-conditioning, q-sampling solver, MBR) for improving their quality.
---

Diffusion models have become a standard approach for generative modeling in continuous domains, yet their application to discrete data remains challenging.
We investigate why Gaussian diffusion models with the DDPM solver struggle to sample from discrete distributions that are represented as a mixture of delta-distributions in the continuous space.
Using a toy Random Hierarchy Model, we identify a critical sampling interval in which the density of noisified data becomes multimodal.
In this regime, DDPM occasionally enters low-density regions between modes producing out-of-distribution inputs for the model and degrading sample quality.
We show that existing heuristics, including self-conditioning and a solver we term q-sampling, help alleviate this issue.
Furthermore, we demonstrate that combining self-conditioning with switching from DDPM to q-sampling within the critical interval improves generation quality on real data.
We validate these findings across conditional and unconditional tasks in multiple domains, including text, programming code, and proteins.
