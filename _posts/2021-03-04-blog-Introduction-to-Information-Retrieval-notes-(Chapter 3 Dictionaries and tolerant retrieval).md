---
title: 'Introduction to Information Retrieval Notes (Chapter 3 Dictionaries and tolerant retrieval)'
date: 2021-03-04
permalink: /posts/2021/03/blog-Information-Retrieval-Notes-Chapter-03/
tags:
  - Information Retrieval
  - Binary Tree
  - Spelling correction
---

**Summary**

- The vocabulary lookup operation uses a classical data structure called the dictionary and has two broad classes of solutions: hashing and search trees. 
- There are some issues for search engines that apply hashing for dictionary lookup: 1. It is difficult to find minor variants of a query term because these could be hashed to very different integers; 2. We cannot seek (for instance) all terms beginning with the prefix, like auto-; 3. In a setting (such as the Web), where the size of the vocabulary keeps growing, a hash function designed for current needs may not suffice in a few years’ time.
- For a balanced tree, the number of comparisons is $O(log M)$. Hence, the principal issue of the search tree is that of rebalancing; as terms are inserted into or deleted from the binary search tree, it needs to be rebalanced so that the balance property is maintained.  
- When applying binary-tree for search engine, unlike hashing search, the document collection must be organized by some prescribed orders, like the alphabet.  
- Using a regular B-tree together with a reverse B-tree, we can handle wildcard queries that contain a single * symbol.
- Two principles for spelling correction: 1. Of various alternative correct spellings for a misspelled query, choose the “nearest” one; 2. The algorithm should choose the more common word as the correction.
- There are two specific forms of spelling correction that is isolated-term correction and context-sensitive correction.
- Isolated-term correction: to correct a single query term at a time, and each term in the query is correctly spelled in isolation. E.g., query *flew form Heathrow*, each word is correct, but *form* should correct to *from*.
- Edit distance and k-gram overlap are two common methods for isolated-term correction.
- Spelling errors do not occur in the first character of the query.
- Zobel and Dart (1995) proposed that k-gram indexing is very effective for finding candidate mismatches but should be combined with a more fine-grained technique such as edit distance to determine the most likely misspellings.   
- Gusfield (1997) is a standard reference on string algorithms such as edit distance.

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-3-Dictionaries-and-tolerant-retrieval.pdf) and [**here**](https://zhuanlan.zhihu.com/p/354542527) to read full blog.
