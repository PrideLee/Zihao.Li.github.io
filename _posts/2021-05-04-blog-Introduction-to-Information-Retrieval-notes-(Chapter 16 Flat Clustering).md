---
title: 'Introduction to Information Retrieval Notes (Chapter 16 Flat Clustering)'
date: 2021-05-04
permalink: /posts/2021/05/blog-Information-Retrieval-Notes-Chapter-16/
tags:
  - Information Retrieval
  - Text clustering
  - KNN
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-16-Flat-Clustering.pdf) and [**here**](https://zhuanlan.zhihu.com/p/368370173) to read full blog.

**Conclusions**

- Finding descriptive labels for clusters automatically is a difficult problem. But cluster-based navigation is an interesting alternative to keyword searching.  This is especially true in scenarios where users prefer browsing over searching because they are unsure about which search terms to use.
- Google News and its precursor, the Columbia NewsBlaster system, are examples of a scatter-gather approach.
- Clustering is well suited for access to a collection of news stories because news reading is not really a search but rather a process of selecting a subset of stories about recent events.
- When computing topic similarity, stop words can be safely ignored, but they are important cues for separating clusters of English (in which the occurs frequently and la infrequently) and French documents (in which the occurs infrequently and la frequently).
- Often, the number of clusters or cardinality of clustering is nothing more than a good guess based on experience or domain knowledge. 
- The scatter-gather interface could not display more than about 10 clusters per layer because of the size and resolution of computer monitors in the early 1990s.
- If the search starts at an unfavorable initial point, we may miss the global optimum. Finding a good starting point is, therefore, another important problem we have to solve in flat clustering.
-  Because deterministic hierarchical clustering methods are more predictable than K -means, hierarchical clustering of a small random sample of size $i$ K (e.g., for $i = 5$ or $i = 10$) often provides good seeds.
- A robust method that works well for a large variety of document distributions is to select $i$ (e.g., $i = 10$) random vectors for each cluster and use their centroid as the seed for this cluster.
- K -means is more efficient than the hierarchical algorithms.
- Distance computations are time-consuming in a naive implementation of K-means. 
- Truncating centroids to the most significant k terms (e.g., k = 1,000) hardly decreases cluster quality while achieving a significant speedup of the reassignment step.
- Euclidean distance and cosine similarity, Kullback-Leibler divergence is often used in clustering as a measure of how (dis)similar documents and clusters are (Xu and Croft 1999; Muresan and Harper 2004; Kurland and Lee 2004).
- Although some of these studies show improvements in effectiveness, efficiency, or both, there is no consensus that cluster-based retrieval works well consistently across scenarios. 
- There is good evidence that clustering of search results improves user experience and search result quality (Hearst and Pedersen 1996; Zamir and Etzioni 1999; Tombros et al. 2002; Kaki 2005; Toda and Kataoka 2005); al- ¨ though not as much as search result structuring based on carefully edited category hierarchies (Hearst 2006). 
- Basu et al. (2004) argue that the three evaluation measures NMI, Rand index, and F measure, give very similar results.
- AIC is due to Akaike (1974) (see also Burnham and Anderson (2002)). An alternative to AIC is BIC, which can be motivated as a Bayesian model selection procedure (Schwarz 1978). 
- Model-based clustering provides a framework for incorporating our knowledge about a domain. 
