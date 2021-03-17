---
title: 'Introduction to Information Retrieval (Chapter 7 Computing scores in a complete search system)'
date: 2021-03-17
permalink: /posts/2021/03/blog-Information-Retrieval-Notes-Chapter-07/
tags:
  - Information Retrieval
  - Score and Raning
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-7-Computing-scores-in-a-complete-search-system.pdf) and [**here**](https://zhuanlan.zhihu.com/p/357535117) to read full blog.

**Summary**
- For cluster, The expected number of followers for each leader is $\approx N /\sqrt N= \sqrt N$.
- Term proximity: Consider a query with two or more query terms, $t1, t2, ... , tk$. Let $\omega$ be the width of the smallest window in a document $d$ that contains all the query terms, measured in the number of words in the window. We could also consider variants in which only words that are not stop words are considered in computing $\omega$.
- Such proximity-weighted scoring functions are a departure from pure cosine similarity and closer to the “soft conjunctive” semantics that Google and other web search engines evidently use.
