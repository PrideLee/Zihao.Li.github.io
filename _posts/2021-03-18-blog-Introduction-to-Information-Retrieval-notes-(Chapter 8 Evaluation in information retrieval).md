---
title: 'Introduction to Information Retrieval Notes (Chapter 8 Evaluation in information retrieval)'
date: 2021-03-18
permalink: /posts/2021/03/blog-Information-Retrieval-Notes-Chapter-08/
tags:
  - Information Retrieval
  - Evaluation
  - Relevance
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-8-Evaluation-in-information-retrieval.pdf) and [**here**](https://zhuanlan.zhihu.com/p/358031013) to read full blog.

**Summary**

- The key utility measure is user happiness. Speed of response and the size of the index are factors in user happiness. It seems reasonable to assume that the relevance of results is the most important factor: blindingly fast, useless answers do not make a user happy. However, user perceptions do not always coincide with system designers’ notions of quality. For example, user happiness commonly depends very strongly on user interface design issues, including the layout, clarity, and responsiveness of the user interface, which are independent of the quality of the results returned.
- The test document collection and suite of information needs have to be of a reasonable size: As a rule of thumb, fifty information needs have usually been found to be a sufficient minimum.
- Accuracy is not an appropriate measure for IR problems since the data are extremely skewed; normally, over 99.9% of the documents are in the nonrelevant category.
- For F measure, values of $\beta < 1$ emphasize precision, whereas values of $\beta > 1$ emphasize recall. 
- Why do we use a harmonic mean rather than the simpler average (arithmetic mean)? The harmonic mean is always less than or equal to the arithmetic mean and the geometric mean. When the values of two numbers differ greatly, the harmonic mean is closer to their minimum than to their arithmetic mean.
- MAP has been shown to have especially good discrimination and stability. 
- Precision at $k$ is the least stable of the commonly used evaluation measures, and that it does not average well because the total number of relevant documents for a query has a strong influence on precision at $k$.
- An ROC curve always goes from the bottom left to the top right of the graph. For a good system, the graph climbs steeply on the left side. 
- At the break-even point: F1 = P = R.
- Maximizing marginal relevance requires returning documents that exhibit diversity and novelty.
- The simplest form of summary takes the first two sentences or fifty words of a document or extracts particular zones of a document, such as a title and an author. 
- In sophisticated NLP approaches, the system synthesizes sentences for a summary, either by doing full-text generation or by editing and perhaps combining sentences used in the document. The last class of methods remains in the realm of research and is seldom used for search results: It is easier, safer, and often even better to just use sentences from the original document.
- Generating snippets must be fast because the system is typically generating many snippets for each query that it handles. Rather than caching an entire document, it is common to cache only a generous but fixed-size prefix of the document, such as perhaps 10,000 characters. 
- Aslam and Yilmaz (2005) examine R-precision surprisingly close correlation to MAP, which had been noted in earlier studies (Tague-Sutcliffe and Blustein 1995; Buckley and Voorhees 2000).
- NDCG is best for evaluating document ranking.
