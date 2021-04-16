---
title: 'Introduction to Information Retrieval Notes (Chapter 13 Text classification and Naive Bayes)'
date: 2021-04-16
permalink: /posts/2021/04/blog-Information-Retrieval-Notes-Chapter-13/
tags:
  - Information Retrieval
  - Text classification
  - Naive Bayes
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-13-Text-classification-and-Naive-Bayes.pdf) and [**here**](https://zhuanlan.zhihu.com/p/364605406) to read full blog.

**Summary**

- A computer is not essential for classification. Many classification tasks have traditionally been solved manually.
- Hand-coded rules have good scaling properties, but creating and maintaining them over time is labor-intensive. 
- Both training and testing complexity are linear in the time it takes to scan the data for NB. Because we have to look at the data at least once, NB can be said to have optimal time complexity. Its efficiency is one reason why NB is a popular text classification method.
- When classifying a test document, the Bernoulli model uses binary occurrence information, ignoring the number of occurrences, whereas the multinomial model keeps track of multiple occurrences. As a result, the Bernoulli model typically makes many mistakes when classifying long documents. 
- NB is also somewhat robust to noise features and concept drift – the gradual change over time of the concept underlying a class like US president from Bill Clinton to George W.
- NB’s main strength is its efficiency: Training and classification can be accomplished with one pass over the data.
- The Bernoulli model is particularly robust with respect to concept drift.
- Classification accuracy often decreases when selecting $k$ common features for a system with $n$ classifiers as opposed to $n$ different sets of size $k$. But even if it does, the gain in efficiency owing to a common document representation may be worth the loss in accuracy.
- $\chi^2$ selects more rare terms (which are often less reliable indicators) than mutual information.
- In most text classification problems, there are a few strong indicators and many weak indicators. As long as all strong indicators and a large number of weak indicators are selected, accuracy is expected to be good. 
- Many practitioners have had the experience of being unable to build a fancy classifier for a certain problem that consistently performs better than NB.
- Although most researchers believe that an SVM is better than kNN and kNN better than NB, the ranking of classifiers ultimately depends on the class, the document collection, and the experimental setup.
- Ng and Jordan (2001) show that NB is sometimes (although rarely) superior to discriminative methods because it more quickly reaches its optimal error rate.
