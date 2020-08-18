---
layout: post
year: 2020
venue: conference paper
title: Scalable Online Monitoring of Distributed Systems

authors: David Basin, Matthieu Gras, Srđan Krstić, Joshua Schneider

details: In the 20th International Conference on Runtime Verification (RV 2020).
pdf: /assets/papers/rv20-multisource.pdf
slides: 
doi: 
bibtex: /assets/papers/rv20-multisource.txt
draft:
repo: https://bitbucket.org/krle/scalable-online-monitor/src/multisource_checkpointing/
artifact: https://github.com/krledmno1/krledmno1.github.io/releases/download/v1.0/multi-source.tar.gz
---

Distributed systems are challenging for runtime verification. Centralized specifications provide a global view of the system, but their semantics requires totally-ordered observations, which are often unavailable in a distributed setting. Scalability is also problematic, especially for online first-order monitors, which must be parallelized in practice to handle high volume, high velocity data streams. We argue that scalable online monitors must ingest events from multiple sources in parallel, and we propose a general model for input to such monitors. Our model only assumes a low-resolution global clock and allows for out-of-order events, which makes it suitable for distributed systems. Based on this model, we extend our existing monitoring framework, which slices a single event stream into independently monitorable substreams. Our new framework now slices multiple event streams in parallel. We prove our extension correct and empirically show that the maximum monitoring latency significantly improves when slicing is a bottleneck.