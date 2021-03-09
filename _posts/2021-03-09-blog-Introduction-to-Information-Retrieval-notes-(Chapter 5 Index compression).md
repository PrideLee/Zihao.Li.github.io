---
title: 'Introduction to Information Retrieval Notes (Chapter 5 Index compression)'
date: 2021-03-09
permalink: /posts/2021/03/blog-Information-Retrieval-Notes-Chapter-05/
tags:
  - Information Retrieval
  - Index compression
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-5-Index-compression.pdf) and [**here**](https://zhuanlan.zhihu.com/p/355299769) to read full blog.

**Summary**

- Compression ratios of 1:4 are easy to achieve, potentially cutting the cost of storing the index by 75%.
- If the main goal of compression is to conserve disk space, then the speed of compression algorithms is of no concern. But for improved cache utilization and faster disk-to-memory transfer, decompression speeds must be high.
- Heaps' law estimates vocabulary size as a function of collection size. $M=kT^b$, where $T$ is the number of tokens in the collection, and $M$ is the vocabulary size. 
- Zipf's law: A commonly used model of the distribution of terms in a collection. $cf_i \propto \frac{1}{i}$.
- For most IR systems, variable byte codes offer an excellent tradeoff between time and space.
- Variable byte codes process queries two times faster than either bit-level compressed indexes or uncompressed indexes with a 30% penalty in compression ratio compared with the best bit-level compression method (Scholer et al. 2002). 
- Compressed indexes can be superior to uncompressed indexes not only in disk usage but also in query processing speed (Scholer et al. 2002).
- Compared with VB codes, "variable nibble" codes showed 5% to 10% better compression and up to one-third worse effectiveness in one experiment (Anh and Moffat 2005).
- Trotman (2003) also recommends using VB codes unless disk space is at a premium. 
- Zhang et al. (2007) investigate the increased effectiveness of caching when a number of different compression techniques for postings lists are used on modern hardware.
- $\delta$ codes and $\gamma$ codes were introduced by Elias (1975), who proved that both codes are universal.
- $\delta$ codes perform better than $\gamma$ codes if large numbers (greater than 15) dominate. 
- Using parameterized codes for index compression, codes that explicitly model the probability distribution of gaps for each term. For example, they show that Golomb codes achieve better compression ratios than $\gamma$ codes for large collections (Witten et al., 1999).
- The distribution of gaps in a postings list depends on the assignment of docIDs to documents.
- Assigning docIDs in a small range to documents in a cluster where a cluster can consist of all documents in a given time period, on a particular website, or sharing another property. As a result, when a sequence of documents from a cluster occurs in a postings list, their gaps are small and can be more effectively compressed.
- Document compression can also be important in an efficient information retrieval system.
