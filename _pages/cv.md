---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======

- **PhD (Computer Science)**: Constructor University, Bremen, Germany, 2024-2026 (expected)
- **MSc (Math of Machine Learning)**: HSE University, Moscow, Russia, 2021-2023 <br>
Thesis title: [Ensembling Neural Networks in the Transfer Learning Setup](https://www.hse.ru/en/ma/sltheory/students/diplomas/836770073)
- **BSc (Applied Mathematics & Informatics)**: HSE University, Moscow, Russia, 2017-2021 <br>
Thesis title: [Empirical Analysis of Self-Supervised Training Properties](https://www.hse.ru/en/edu/vkr/470558018)

**Languages:** Russian (native), English (C1)

Work experience
======

- [**Centre of Deep Learning and Bayesian Methods**](https://bayesgroup.ru/) &mdash;
HSE University, Moscow, Russia, 2021-2023 <br>
*Research assistant*: Fundamental research in deep learning
- [**SmartDec**](https://smartdec.net) &mdash; Moscow, Russia, 2019-2020 <br>
*Intern, development & analytics*: Industrial research in cryptography and zero-knowledge proofs

Skills
======
* **Programming languages**:
  * *Proficient*: Python, LaTeX
  * *Intermediate*: C/C++, Rust
* **Technologies**:
  * *Data science:* PyTorch, NumPy, Pandas, scikit-learn, matplotlib
  * *Linux*: bash, git, ssh, docker

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
