---
layout: post
year: 2020
venue: conference paper
title: Scalable Online Monitoring of Distributed Systems

authors: Joshua Schneider, David Basin, Frederik Brix, Srđan Krstić, Dmitriy Traytel

details: Submitted to the 20th International Conference on Runtime Verification (RV 2020).
pdf: /assets/papers/rv20-multisource.pdf
slides: 
doi: 
bibtex: /assets/papers/rv20-multisource.txt
draft: true
repo: https://bitbucket.org/krle/scalable-online-monitor/src/multisource_checkpointing/
---

Distributed systems are challenging for runtime verification. Centralized specifications admit a global view of the system, but their semantics assumes totally-ordered observations, which are often unavailable in a distributed setting. Scalability is also problematic, especially for online first-order monitors, which must be parallelized in practice to handle the complexity of monitoring first-order specifications. We argue that scalable online monitors must ingest events from multiple sources in parallel, and propose a general model for the input of such monitors. Our model only assumes a finitely-precise global clock and allows out-of-order events, which makes it suitable for distributed systems. Based on this model, we extend our previous monitoring framework, which slices a single event stream into independently monitorable substreams. Our new framework receives events from multiple sources and slices them in parallel. We prove our extension correct and empirically show that the maximum monitoring latency significantly improves in situations where slicing was previously a bottleneck.
