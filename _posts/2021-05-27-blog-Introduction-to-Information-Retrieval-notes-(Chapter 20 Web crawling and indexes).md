---
title: 'Introduction to Information Retrieval Notes (Chapter 20 Web crawling and indexes)'
date: 2021-05-27
permalink: /posts/2021/05/blog-Information-Retrieval-Notes-Chapter-20/
tags:
  - Information Retrieval
  - Web search
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-20-Web-crawling-and-indexes.pdf) and [**here**](https://zhuanlan.zhihu.com/p/375609065) to read full blog.

**Conclusions**
- As a reference point, fetching a billion pages (a small fraction of the static Web at present) in a month-long crawl requires fetching several hundred pages each second. 
- DNS resolution is a well-known bottleneck in web crawling.
- A standard remedy is to introduce caching: URLs for which we have recently performed DNS lookups are likely to be found in the DNS cache, avoiding the need to go to the DNS servers on the Internet. 
- The first web crawler appears to be Matthew Gray’s Wanderer, written in the spring of 1993.
- The designers of Mercator recommend a rough rule of three times as many back queues as crawler threads.
