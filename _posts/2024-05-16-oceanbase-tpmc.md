---
layout: post
title: "[reading review] OceanBase: A 707 Million tpmC Distributed Relational Database System"
date: 2024-05-15 15:16:00
description: reading review
tags: database
categories: reading-reviews
---

In this paper, the authors designed and implemented a distributed relational database, OceanBase, which get the 1st place in the TPC-C benchmark. It is a shared-nothing architecture and can scale out with multiple tenent. Oceanbase has a LSM Tree Basestorage architecture and implements paxos groups to achieve high data reliability and service availability.

- **Strengths**: native distributed architecture, no need for database middleware; high data reliability and service availability.

- **Future works**: improve query optimization ability for complex SQL statements.
