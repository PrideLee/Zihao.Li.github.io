---
title: 'Graph Neural Networks in Recommender Systems: A Survey'
date: 2021-06-19
permalink: /posts/2021/06/blog-Graph-Neural-Networks-in-Recommender-Systems-A-Survey/
tags:
  - Recommendation
  - Graph Neural Network
  - Sequential recommendation
---

You can click [**here**](https://pridelee.github.io/files/blog/Graph-Neural-Networks-in-Recommender-Systems-A-Survey.pdf) and [**here**](https://zhuanlan.zhihu.com/p/382103093) to read full blog.

**Conclusions**
- In fact, using collaborative signals to improve representation learning in recommender systems is not a new idea that originated from GNN. Early eﬀorts, such as SVD++ and FISM, have already demonstrated the eﬀectiveness of the interacted items in user representation learning.
- There exist comprehensive surveys on
recommender systems ([Quadrana, *et al.*](https://arxiv.org/pdf/1802.08452.pdf); [S Zhang, *et al.*](https://arxiv.org/pdf/1707.07435.pdf)) or graph neural networks ([Z Wu, *et al.*](https://arxiv.org/pdf/1901.00596.pdf); [J Zhou, *et al.*](https://arxiv.org/ftp/arxiv/papers/1812/1812.08434.pdf)).
- According to whether the users are anonymous or not and whether the behaviors are segmented into sessions, works in this field can be further divided into sequential recommendation and session-based recommendation. The session-based recommendation can be viewed as a sub-type of sequential recommendation with anonymous and session assumptions. 
- Sampling is a trade-oﬀ between the original graph information and computational efficiency. The PinSage includes more randomness while IG-MC sacrifices more graph information. In terms of transferring, the sampling method of IG-MC is preferable; otherwise, the strategy of PinSage might be better.
- Note that some works observe that nonlinear activation contributes little to the overall performance, and they simplify the update operation by removing the non-linearities, thereby retaining or even improving performance and increasing computational efficiency.
- In most scenarios, the length of the user sequence is short, e.g., the average length on the preprocessed Yoochoose$1/4^2$ dataset is 5.71.
