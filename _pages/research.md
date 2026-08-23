---
layout: page
permalink: /research/
title: research
nav: true
nav_order: 1
description: Research on coded distributed computing, elastic systems, and efficient AI inference.
---

## Coded Elastic Computing

Distributed computing systems must often operate with workers whose speeds, storage resources, and availability change over time. My research develops coded and uncoded-storage schemes that make distributed matrix computation resilient to **stragglers** and **dynamic worker availability**, while adapting computation assignments to heterogeneous resources.

Key themes include Lagrange-coded computation, storage and download design, straggler tolerance, heterogeneous computation assignment, and practical evaluation in cloud environments.

## Distributed Aggregation and Function Computation

I study how coded computation can recover a desired aggregate function directly, rather than first recovering every intermediate result. This line of work characterizes **feasibility and recovery limits under straggler patterns** and develops explicit coded constructions that achieve those limits.

## Communication-Efficient Distributed and Edge Computing

A current direction of my work is to jointly account for **download, computation, and upload latency** when communication resources are shared. I am interested in how coding, bandwidth allocation, storage placement, and computation assignment interact in heterogeneous edge systems.

## Efficient AI Inference

I am exploring the application of coding and compression ideas to modern AI inference systems, especially **transformer inference at the edge**. Topics of current interest include KV-cache compression, quantization, attention/softmax-aware error analysis, and communication-efficient distributed inference.

This is an emerging research direction for me; my published work to date is primarily in coded computing, distributed computation, and coded caching.
