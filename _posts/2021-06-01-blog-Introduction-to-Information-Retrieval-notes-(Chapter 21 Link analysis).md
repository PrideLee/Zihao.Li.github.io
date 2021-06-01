---
title: 'Introduction to Information Retrieval Notes (Chapter 21 Link analysis)'
date: 2021-06-01
permalink: /posts/2021/06/blog-Information-Retrieval-Notes-Chapter-21/
tags:
  - Information Retrieval
  - PageRank
  - Link analysis
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-21-Link-analysis.pdf) and [**here**](https://zhuanlan.zhihu.com/p/375612557) to read full blog.

**Conclusions**
- Link analysis for web search has intellectual antecedents in the field of citation analysis, aspects of which overlap with an area known as bibliometrics.
- Because the iterative updates captured the intuition of good hubs and good authorities, the high-scoring pages we output would give us good hubs and authorities from the target subset of web pages.
- Ng et al. (2001b) suggest that the PageRank score assignment is more robust than HITS in the sense that scores are less sensitive to small changes in a graph topology. However, it has also been noted that the teleport operation contributes significantly to PageRank’s robustness in this sense. 
- Ng et al. (2001b) introduce a notion of stability for link analysis, arguing that small changes to link topology should not lead to significant changes in the ranked list of results for a query. 
