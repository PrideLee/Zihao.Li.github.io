---
title: 'Introduction to Information Retrieval Notes (Chapter 17 Hierarchical Clustering)'
date: 2021-05-08
permalink: /posts/2021/05/blog-Information-Retrieval-Notes-Chapter-17/
tags:
  - Information Retrieval
  - Text clustering
  - Hierarchical clustering
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-17-Hierarchical-clustering.pdf) and [**here**](https://zhuanlan.zhihu.com/p/369749913) to read full blog.

**Conclusions**

- In general, we select flat clustering when efficiency is important and hierarchical clustering when one of the potential problems of flat clustering (not enough structure, predetermined number of clusters, nondeterminism) is a concern. In addition, many researchers believe that hierarchical clustering produces better clusters than flat clustering. 
- Hierarchical clustering does not require us to prespecify the number of clusters, and most hierarchical algorithms that have been used in information retrieval (IR) are deterministic.
- The most common hierarchical clustering algorithms have a complexity that is at least quadratic in the number of documents compared to the linear complexity of K-means and EM.
- HAC is more frequently used in IR than top-down clustering.
- The complexity of the naive HAC algorithm is $O(N^3)$ because we exhaustively search the $N \times N$ matrix $C$ for the largest similarity in each of $N − 1$ iterations.
- Top-down clustering is conceptually more complex than bottom-up clustering; we need a second, flat clustering algorithm as a “subroutine.” It has the advantage of being more efficient if we do not generate a complete hierarchy all the way down to individual document leaves. For a fixed number of top levels, using an efficient flat algorithm like K-means, top-down algorithms are linear in the number of documents and clusters. So they run much faster than HAC algorithms, which are at least quadratic.
- There is evidence that divisive algorithms produce more accurate hierarchies than bottom-up algorithms in some circumstances. 
- Top-down clustering benefits from complete information about the global distribution when making top-level partitioning decisions.
- A combination of a differential test with a penalty for rare terms often gives the best labeling results because rare terms are not necessarily representative of the cluster as a whole.
- Cluster-internal methods are efficient, but they fail to distinguish terms that are frequent in the collection as a whole from those that are frequent only in the cluster. 
- For large vocabularies, complete-link clustering can be more efficient than an unoptimized implementation of GAAC.
- Even with these optimizations, HAC algorithms are all $O(N^2)$ or $O(N^2 log N)$ and therefore infeasible for large sets of 1,000,000 or more documents. For such large sets, HAC can only be used in combination with a flat clustering algorithm like K-means. 
- We can employ a HAC algorithm to compute seeds of high quality for K-Menas. This algorithm is referred to as the Buckshot algorithm. It combines the determinism and higher reliability of HAC with the efficiency of K-means.
- There is no doubt that results of EM and K-means are highly variable since they will often converge to a local optimum of poor quality. The HAC algorithms we have presented here are deterministic and thus more predictable.
- Ward’s method (Ward Jr. 1963; El-Hamdouchi and Willett 1986), also called minimum variance clustering. In each step, it selects the merge with the smallest RSS. The merge criterion in Ward’s method (a function of all individual distances from the centroid) is closely related to the merge criterion in GAAC (a function of all individual similarities to the centroid).
- Despite its importance for making the results of clustering useful, comparatively little work has been done on labeling clusters.
- Some clustering algorithms attempt to find a set of labels first and then build (often overlapping) clusters around the labels, thereby avoiding the problem of labeling altogether (Zamir and Etzioni 1999; Kaki 2005; ¨ Osinski and Weiss 2005). 
- An example of an efficient divisive algorithm is bisecting K-means (Steinspectral bach et al. 2000). Spectral clustering algorithms (Kannan et al. 2000; Dhillon 2001; Zha et al. 2001; Ng et al. 2001a), including principal direction divisive partitioning (PDDP) (whose bisecting decisions are based on SVD, see Chapter 18) (Boley 1998; Savaresi and Boley 2004), are computationally more expensive than bisecting K -means, but have the advantage of being deterministic.
- Unlike K-means and EM, most hierarchical clustering algorithms do not have a probabilistic interpretation. Model-based hierarchical clustering (Vaithyanathan and Dom 2000; Kamvar et al. 2002; Castro et al. 2004) is an exception.
