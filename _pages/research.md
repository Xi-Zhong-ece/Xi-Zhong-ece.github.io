---
layout: page
permalink: /research/
title: research
description: Research directions in coded computing, distributed systems, and efficient AI inference.
nav: true
nav_order: 1
---

## Distributed Aggregation and Function Computation

I develop coded methods for computing aggregate functions directly in distributed systems under stragglers, without unnecessarily recovering every individual intermediate result. My recent work establishes fundamental feasibility and recovery limits through necessary and sufficient conditions and explicit constructions.

## Elastic and Heterogeneous Distributed Computing

I study distributed systems in which workers may have heterogeneous computation speeds, storage capacities, and dynamic availability. My work develops computation-assignment and coding schemes that jointly address **heterogeneity, elasticity, and stragglers**, with both theoretical performance guarantees and system-level evaluation on AWS EC2.

Topics include:

- coded elastic computing and Lagrange-coded computation,
- coded and uncoded storage/download strategies,
- computation and communication tradeoffs,
- straggler tolerance and dynamic worker availability,
- latency-aware computation assignment.

## Efficient AI Inference

I am currently exploring how ideas from coding, compression, and distributed optimization can be applied to efficient AI inference. In particular, I am interested in **communication-efficient edge inference, transformer inference, KV-cache compression, quantization, and attention-aware compression**.

This is an emerging research direction that builds on my background in information theory and distributed computing.

## Earlier Work: Coded Caching

My earlier research studied coded caching and content delivery, with an emphasis on reducing subpacketization and implementation complexity while preserving coding gains.
