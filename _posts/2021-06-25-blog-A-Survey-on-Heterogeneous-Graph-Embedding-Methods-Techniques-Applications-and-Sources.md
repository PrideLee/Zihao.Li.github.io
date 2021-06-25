---
title: 'A Survey on Heterogeneous Graph Embedding: Methods, Techniques, Applications and Sources'
date: 2021-06-25
permalink: /posts/2021/06/blog-A-Survey-on-Heterogeneous-Graph-Embedding-Methods-Techniques-Applications-and-Sources/
tags:
  - Heterogeneous Graph
  - Embedding
  - Survey
---

You can click [**here**](https://pridelee.github.io/files/blog/A-Survey-on-Heterogeneous-Graph-Embedding-Methods-Techniques-Applications-and-Sources.pdf) and [**here**](https://zhuanlan.zhihu.com/p/383954921) to read full blog.

**Conclusions**
- Most message passing-based methods have the inductive capability because they can update the node embeddings by aggregating neighborhood information. But they need additional labels to guide the training process.
- Most deep learning-based methods are proposed for HG with attributes or a specific application, while the shallow model-based methods are mainly designed for the use of structures.
- The emerging HGNNs can naturally integrate graph structures and attributes, so it is more suitable for the complex scenes and content.
- Shallow models are easy to parallel. But they are two-stage training, i.e., the embeddings are not relevant to the downstream tasks, and the memory cost is heavy. On the contrary, deep models are end-to-end training and require less memory space. 
- Message passing-based techniques are good at encoding structures and attributes simultaneously and integrating different semantic information. 
- Compared with message passing-based techniques, encoder-decoder-based techniques are weak in fusing information due to the lack of messaging mechanism. But they are more flexible to introduce different objective functions through different decoders.
- Adversarial-based methods prefer to utilize the negative samples to enhance the robustness of the embeddings. But the choice of negative samples has a huge influence on the performance, thus leading to higher variances.
- The complexity of the random walk technique consists of two parts: random walk and skip-gram, both of which are linear with the number of nodes. 
- Decomposition technique needs to divide HGs into sub-graphs according to the type of edges, so the complexity is linear with the number of edges, which is higher than a random walk. 
- Message passing technique mainly uses node-level and semantic-level attention to learn node embeddings, so its complexity is related to the number of nodes and node types.
- As for the encoder-decoder technique, the complexity of the encoder is related to the number of nodes, while the decoder is usually used to preserve the network structures, so it is linear with the number of edges. 
- Adversarial technique needs to generate the negative samples for each node, so the complexity is related to the number of nodes and negative samples.
