---
layout: splash
permalink: /
title: "Cam-BIO"
header:
  overlay_color: "#2a5490"
  overlay_filter: "0.55"
  overlay_image: /assets/images/deckphoto.JPG
  actions:
    - label: "Explore Features"
      url: /features/
    - label: "View on GitHub"
      url: https://github.com/cdsnow
excerpt: >-
  A voice-controlled AI lab assistant for the OpenTrons Flex: describe your
  experiment out loud and it designs protocols collaboratively with a user.
intro:
  - excerpt: >-
        Cam-BIO is an open source human-AI collaboration platform designed to speed up the next generation of benchtop experiments at Colorado State University. With the advent of automated design pipelines powered by large-scale prediction models such as Alphafold3, Boltz-2, RFdiffusion and others, experimental workloads for validating machine learning outputs have yet to catch up. We on the Cam-BIO team aim to bring automated experimental protocols to CSU's researchers in an open-source, validated, and easy-to-use manner to bridge this knowledge gap, as well as speeding up other laboratory experimentation such as PCR, protein crystalization, and directed evolution. 
feature_row:
  - title: "Talk to your robots"
    excerpt: >-
      We plan to have a conversational interface agent for all a wide variety of laboratory robots all managed by a Director AI. The first one, Cam, is an OpenTrons Flex agent features a voice interface that builds liquid handling protocols with from a conversation with a human. You can speak to Cam and ask clarifying questions about a protocol, ask it for information the FLEX, and ask it to run preapproved protocols. 
  - title: "Plan experiments collaboratively"
    excerpt: >-
      Director agent who sees all robots and inventory and can plan based on current capabilities.
  - title: "Keep track of results and inventory"
    excerpt: >-
      Inventory agent
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}
