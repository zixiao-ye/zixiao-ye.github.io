---
layout: post
title: "[reading review] The FastLanes Compression Layout: Decoding >100 Billion Integers per Second with Scalar Code"
date: 2024-06-06 17:30:00
description: reading review
tags: database layout
categories: reading-reviews
---

In this paper, the authors propose a new layout FastLanes to accelerate decoding speed. FastLanes is designed to adapt to many heterogeneous ISAs and can also run on a virtual 1024-bits register. Because relational algebra is based on set concept, the authors can reorder data to vectorize the query execution process without harm the performance. Another notable result is that modern compiler can do auto-vectorize the scalar FastLanes layout code without explicit SIMD intrinsics.

- **Strengths**: By reordering data and design a virtual 1024-bits register, FastLanes can leverage SIMD to accelerate decoding process and portable to many different existing ISAs.

- **Future works**: One can integrate FastLanes to a complete system to evaluate performace and do more experiments on GPUs and TPUs.