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
  - title: "Talk to your robots"
    excerpt: >-
      We are building conversational agents for a wide variety of laboratory robots, all coordinated by a director AI. Our first robot agent, Robert, drives the OpenTrons Flex with a voice interface that builds liquid handling protocols from a conversation with a human. You can ask Robert clarifying questions about a protocol, ask it for information about the Flex, and request it to run preapproved protocols. In protocol planning mode, Robert and a human user work together to write the protocol code for a desired experiment.
  - title: "Plan experiments collaboratively"
    excerpt: >-
      Cam, our director agent, sees every robot and the lab's inventory, and works with you to plan experiments that span multiple instruments based on what the lab can do right now.
  - title: "Keep track of results and inventory"
    excerpt: >-
      Iven, our inventory agent, keeps track of your lab's inventory and reports back to the user and director when supplies are low, or simply where they are located in the lab space! Iven's job is also to keep track of technical documents and result files.
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}
