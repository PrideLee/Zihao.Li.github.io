---
title: 'Introduction to Information Retrieval Notes (Chapter 18 Matrix decompositions and latent semantic indexing)'
date: 2021-05-12
permalink: /posts/2021/05/blog-Information-Retrieval-Notes-Chapter-18/
tags:
  - Information Retrieval
  - Matrix decompositions
  - SVD & LSA
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-18-Matrix-decompositions-and-latent-semantic-indexing.pdf) and [**here**](https://zhuanlan.zhihu.com/p/370761772) to read full blog.

**Conclusions**
- Although latent semantic indexing has not been established as a significant force in scoring and ranking for information retrieval (IR), it remains an intriguing approach to clustering in a number of domains, including for collections of text documents.
- The effect of small eigenvalues (and their eigenvectors) on a matrix-vector product is small.
- For a symmetric matrix $S$, the eigenvectors corresponding to distinct eigenvalues are orthogonal. Further, if $S$ is both real and symmetric, the eigenvalues are all real.
- For LSI, in the experimental work cited, $k$ is generally chosen to be in the low hundreds. 
- The quality of the LSI representation will degrade as more documents are added and will eventually require recomputation of the LSI representation.
- The fidelity of the approximation of $C_k$ to $C$ leads us to hope that the relative values of cosine similarities are preserved: if a query is close to a document in the original space, it remains relatively close in the k-dimensional space. But this in itself is not sufficiently interesting, especially given that the sparse query vector $\overrightarrow q$ turns into a dense query vector $\overrightarrow q_k$ in the low-dimensional space. 
- Dumais (1993) and Dumais (1995) conducted experiments with LSI on TREC documents and tasks, using the commonly used Lanczos algorithm to compute the SVD. At the time of their work in the early 1990s, the LSI computation on tens of thousands of documents took approximately one day on one machine. In these experiments, they achieved precision at or above that of the median TREC participant. In about 20% of TREC topics, their system was the top scorer and reportedly slightly better on average than standard vector spaces for LSI at about 350 dimensions. Here are some conclusions on LSI first suggested by their work and subsequently verified by many other experiments.
