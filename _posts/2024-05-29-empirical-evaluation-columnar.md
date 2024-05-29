---
layout: post
title: "[reading review] An Empirical Evaluation of Columnar Storage Formats"
date: 2024-05-29 06:00:00
description: reading review
tags: database columnar
categories: reading-reviews
---

In this paper, the authors revisted the most popular columanr storage formats (Parquet and ORC). They evaluated these two formats in encoding, compression, index and filter and decoding, etc. The authors also designed a benchmark to fully explore the performance of both formats. Looking deeply into the experimnets results, we can get some useful thoughts on how to design new columnar format.

- **Strengths**: When desgining columnar storage formats, we should keep in mind: It is important to adopt simple encoding scheme for decoding speed.

- **Future works**: New columnar format should consider more about how to use GPU for accelerating and how to leverage the high bandwidth, high latency cloud environment.
