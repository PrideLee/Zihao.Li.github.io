---
title: 'Introduction to Information Retrieval Notes (Chapter 1 Boolean Retrieval)'
date: 2021-03-01
permalink: /posts/2021/03/blog-Information-Retrieval-Notes-Chapter-01/
tags:
  - Information Retrieval
  - Inverted Index
  - Web Search
---

## [Introduction to Information Retrieval](https://nlp.stanford.edu/IR-book/information-retrieval-book.html) notes (Chapter 1 Boolean Retrieval). 

### Summary

- Information retrieval (IR) is finding material (usually documents) of an unstructured nature (usually text) that satisfies an information need from within large collections (usually stored on computers). 
-  The main application scenarios of IR include web search; enterprise, institutional, and domain-specific search; and personal information retrieval.
- The speed of IR, Matching operations, and Ranking accuracy are the main focuses of web-scale information retrieval.
- Incidence Matrix is an intuitive method for information retrieval, and the bitwise operation can be applied for a query search. But the matrix is high-dimensional and sparse.
- Inverted index: an index always maps index back from terms to the parts of a document where they occur.
- Suppose the lengths of the postings lists are $x$ and $y$ (postings lists should be sorted by a single global ordering), the intersection operation could be accomplished by scanning the lists only once. Thus, the $and$ and $not \; and$ operations take $O(x + y)$ operations, and the intersection time is linear in the number of documents and query terms.
- In the case of $AND$ operator, the complexity of merging the postings list depends on the length of the shorter postings list. Therefore, the more short the smaller postings list, the lesser the time spent.
- There is a trade-off between $AND$ and $OR$ operation for information retrieval since the $AND$ may increase the accuracy of results while impairing the recall, vise versa.

You can click [**here**](https://pridelee.github.io/files/blog/Chapter1-Boolean-retrieval.pdf) and [**here**](https://zhuanlan.zhihu.com/p/353850769) to read full blog.
