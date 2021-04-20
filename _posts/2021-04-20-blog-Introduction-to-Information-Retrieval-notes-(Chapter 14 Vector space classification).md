---
title: 'Introduction to Information Retrieval Notes (Chapter 14 Vector space classification)'
date: 2021-04-20
permalink: /posts/2021/04/blog-Information-Retrieval-Notes-Chapter-14/
tags:
  - Information Retrieval
  - Text classification
  - Rocchio classification & knn classification
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-14-Vector-space-classification.pdf) and [**here**](https://zhuanlan.zhihu.com/p/365443226) to read full blog.

**Summary**

- To respecting contiguity, the classes in Rocchio classification must be approximate spheres with similar radii. 
- Unweighted and unnormalized counts should not be used in vector space classification.
- Rocchio classification is simple and efficient but inaccurate if classes are not approximately spheres with similar radii.
- If the training set is large, then kNN can handle nonspherical and other complex classes better than Rocchio.
- A large number of text classifiers can be viewed as linear classifiers – classifiers that classify based on a simple linear combination of the features.
- Because of the bias-variance tradeoff, more complex nonlinear models are not systematically better than linear models. 
- Nonlinear models have more parameters to fit on a limited amount of training data and are more likely to make mistakes for small and noisy data sets.
- For $k$ nearest neighbor, it is desirable for $k$ to be odd to make ties less likely. k = 3 and k = 5 are common choices, but much larger values, between 50 and 100, are also used. 
- For $k$ nearest neighbor, weighting by similarities is often more accurate than simple voting
- The error of 1NN is asymptotically (as the training set increases) bounded by twice the Bayes error rate. That is, if the optimal classifier has an error rate of $x$, then 1NN has an asymptotic error rate of $2x$. This is due to the effect of noise. 
- Naive Bayes and Rocchio – are instances of linear classifiers, the perhaps most important group of text classifiers.
- Bias is small if (i) the classifiers are consistently right or (ii) different training sets cause errors on different documents, or (iii) different training sets cause positive and negative errors on the same documents, but that average out to close to 0. 
- We can also think of variance as the model complexity or, equivalently, memory capacity of the learning method – how detailed a characterization of the training set it can remember and then apply to new data.
