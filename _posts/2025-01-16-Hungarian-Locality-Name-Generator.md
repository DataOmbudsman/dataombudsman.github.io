---
title: Hungarian Locality Name Generator
date: 2025-01-16 08:35:00 +0100
categories: [app]
tags: [github, python, streamlit, machine learning]   # TAG names should always be lowercase
description: An LSTM implementation
---

[![HUNGenerator illustration](/assets/images/posts/hungenerator/HU_counties_blank.svg.png)](https://hungenerator.streamlit.app/){: style="display: block; margin: auto; border: 0px solid #ccc; border-radius: 4px; max-width: 70%;"}

I've always found city and village names fascinating—they feel like they hold hidden meanings that regular words don't. So I wanted to see if I could generate entirely new locality names that don't exist but still sound authentic. To do this, I trained a character-based LSTM on all ~3,100 Hungarian locality names and wrapped it in a Streamlit app so others could experiment with it as well.  

It was a fun project to practice PyTorch, and one discovery was that undertrained networks generated far more entertaining names. My personal favorites are Tokonya and Balatonhalász. Check out the app [here](https://hungenerator.streamlit.app/) and its repo [here](https://github.com/DataOmbudsman/locality-name-generator).
