---
title: 'Introduction to Information Retrieval Notes (Chapter 12 Language models for information retrieval)'
date: 2021-04-08
permalink: /posts/2021/04/blog-Information-Retrieval-Notes-Chapter-12/
tags:
  - Information Retrieval
  - Languag Model
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-12-Language-models-for-information-retrieval.pdf) and [**here**](https://zhuanlan.zhihu.com/p/363006337) to read full blog.

## Conclusions
- Providing that the stop probability is fixed, its inclusion will not alter the likelihood ratio that results from comparing the likelihood of two language models generating a string. 
- Most language-modeling work in IR has used unigram language models. 
- Unigram models are often sufficient to judge the topic of a text. 
- With limited training data, a more constrained model tends to perform better. In addition, unigram models are more efficient to estimate and apply than higher order models.
- Ponte and Croft (1998) argued strongly for the effectiveness of the term weights that come from the language modeling approach over traditional tf–idf weights.
- Much recent work has recognized the importance of document length normalization. 
- The effect of doing a mixture of document generation probability with collection generation probability is a little like idf; terms rare in the general collection but common in some documents will have a greater influence on the ranking of documents.
- Recent work has shown the LM approach to be very effective in retrieval experiments, beating tf–idf and BM25 weights.
- Lafferty and Zhai (2001) present results suggesting that a model comparison approach outperforms both query-likelihood and document-likelihood approaches. 
- Zhai and Lafferty (2002) argue that a two-stage smoothing model with first Bayesian smoothing followed by linear interpolation gives a good model of the task, and performs better and more stably than a single form of smoothing. 
- Liu and Croft (2004) show some gains by smoothing a document LM with estimates from a cluster of similar documents; Tao et al. (2006) report larger gains by doing documentsimilarity based smoothing.
- Sparck Jones (2004) presents a critical viewpoint on the rationale for the language modeling approach, but Lafferty and Zhai (2003) argue that a unified account can be given of the probabilistic semantics underlying both the LM approach presented and the classical probabilistic information retrieval approach. 
