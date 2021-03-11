---
title: 'Introduction to Information Retrieval (Chapter 6 Scoring, term weighting, and the vector space model)'
date: 2021-03-11
permalink: /posts/2021/03/blog-Information-Retrieval-Notes-Chapter-06/
tags:
  - Information Retrieval
  - TF-IDF
  - Text retrieval
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-6-Scoring-term-weighting-and-the-vector-space-model.pdf) and [**here**](https://zhuanlan.zhihu.com/p/356108470) to read full blog.

**Summary**

- A very standard weighting scheme is lnc.ltc, where the document vector has log-weighted term frequency, no idf (for both effectiveness and efficiency reasons), and cosine normalization, while the query vector uses log-weighted term frequency, idf weighting, and cosine normalization.
