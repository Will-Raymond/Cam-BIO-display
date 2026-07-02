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
        Cam-BIO is a human-AI collaboration platform designed to speed up the next generation of benchtop experiments at Colorado State University. With the advent of automated design pipelines powered by large-scale prediction models such as Alphafold3, Boltz-2, RFdiffusion and others, experimental workloads for validating machine learning outputs have yet to catch up. We on the Cam-BIO team aim to bring automated experimental protocols to CSU's researchers in an open-source, validated, and easy-to-use manner. 
feature_row:
  - title: "Talk to your robot"
    excerpt: >-
      A conversational voice interface (speech-to-text + text-to-speech) that
      greets you, asks clarifying questions, confirms assumptions, and narrates
      what it's about to do — before it does it.
  - title: "Sees the deck"
    excerpt: >-
      A camera + vision pipeline that reads the deck: identifying labware,
      detecting tip presence, and recognizing returning users — keeping an
      always-current picture of what's loaded where.
  - title: "Knows your protocols"
    excerpt: >-
      A searchable protocol library with rich, LLM-ready metadata, plus live
      inventory of tips, tubes, and pipettes with confidence that decays over
      time so stale assumptions get re-checked.
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}
