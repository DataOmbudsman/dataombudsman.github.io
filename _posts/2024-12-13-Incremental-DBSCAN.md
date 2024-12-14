---
title: Incremental DBSCAN clustering
date: 2024-12-14 16:35:00 +0100
categories: [package]
tags: [github, python, machine learning, clustering]   # TAG names should always be lowercase
description: A Python implementation
---

[![Custering illustration](/assets/images/posts/incdbscan/clustering.png)](https://github.com/DataOmbudsman/incdbscan){: style="display: block; margin: auto; border: 1px solid #ccc; border-radius: 4px; padding: 4px; max-width: 80%;"}

I authored `incdbscan`, the open source implementation of IncrementalDBSCAN clustering as a Python package, after facing a problem at work. At LogMeIn, we wanted to cluster chat messages and were wondering if the clustering could be easily updated with adding new messages or removing old ones. DBSCAN had been working well for our clustering needs, so we started looking for an incremental version. Although the authors of DBSCAN described an algorithm called IncrementalDBSCAN in a [1998 paper](https://www.dbs.ifi.lmu.de/Publikationen/Papers/VLDB-98-IncDBSCAN.pdf), no public implementation seemed to exist.

`incdbscan` became my COVID project. Implementing the algorithm turned out to be longer and more challenging than expected. The paper had a few gaps that forced me to rethink parts of the algorithm, handle tricky edge cases, and thoroughly test the implementation with unit tests. It was also a great chance to dive into tools and processes like line profiling, publishing to PyPI, and setting up pipelines with GitHub Actions.

As of December 2024, incdbscan has grown in popularity, with about 1,500 monthly downloads according to [PyPI Stats](https://pypistats.org/packages/incdbscan).

![Download stats](/assets/images/posts/incdbscan/downloads.png){: style="display: block; margin: auto; border: 1px solid #ccc; border-radius: 4px; padding: 4px; "}

You can find the code and usage examples here: [https://github.com/DataOmbudsman/incdbscan](https://github.com/DataOmbudsman/incdbscan)

This work was also [presented](https://budapestml.hu/download/budapestml22/fulop_arpad_rollbar.pdf) at the Budapest ML Forum and at a PyData Budapest meetup.
