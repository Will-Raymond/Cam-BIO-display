---
layout: splash
permalink: /
title: "Cam-BIO"
header:
  overlay_color: "#2a5490"
  overlay_filter: "0.55"
  overlay_image: /assets/images/deckphoto.JPG
  actions:
    - label: "Meet our Agents"
      url: /equipment/
    - label: "View on GitHub"
      url: https://github.com/cdsnow
excerpt: >-
  A library of voice-controlled AI lab assistants for various automated experiment platforms. Describe your
  experiments out loud and our agents design protocols collaboratively with a user for their robots.
intro:
  - excerpt: >-
        Cam-BIO is an open source human-AI collaboration platform designed to speed up the next generation of benchtop experiments at Colorado State University. With the advent of automated design pipelines powered by large-scale prediction models such as Alphafold3, Boltz-2, RFdiffusion and others, experimental workloads for validating machine learning outputs have yet to catch up. We on the Cam-BIO team aim to bring automated experimental protocols to CSU's researchers in an open-source, validated, and easy-to-use manner to bridge this knowledge gap, as well as speeding up other laboratory experimentation such as PCR, protein crystalization, and directed evolution. 
feature_row:
  - title: "Lowering the activation energy to lab automation"
    excerpt: >-
      Lab automation shouldn't be locked behind 12 APIs and 3 months of finagling. At Cam-BIO we are enabling large scale automated protocols at Colorado State University and beyond. Talk directly to Cam, our collaborative lab director agent, to design and dispatch experimental protocols across multiple machines throughout the lab space. Cam will guide you through collecting the materials and results and store them for you, iterating on the protocol with you for flexibility, optimality, and ease of use.
  - title: "You are looped in on a lab-in-the-loop"
    excerpt: >-
      (in development) A Lab in the loop approach lets the individual robot agents report back and summarize results and runs as well as troubleshoot automatically for you. Cam stores all runs are stored in a searchable, historical database for you to view what worked, what didn't, and where to go next. Our agents learn on your protocols to reduce iteration time and errors.
  - title: "A robust library of experiments"
    excerpt: >-
      We are building high throughput protocols for automated PCR, automated protein crystalization, directed evolution, protein purification, oligonucleotide library assembly, and more!
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}
