---
title: 'Introduction to Information Retrieval Notes (Chapter 3 Dictionaries and tolerant retrieval)'
date: 2021-03-04
permalink: /posts/2021/03/blog-Information-Retrieval-Notes-Chapter-03/
tags:
  - Information Retrieval
  - Binary Tree
  - Spelling correction
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-3-Dictionaries-and-tolerant-retrieval.pdf) and [**here**](https://zhuanlan.zhihu.com/p/358986119) to read complete blog.

**Summary**

- Relevance feedback is one of the most used and most successful approaches for synonymy problems.
- Relevance feedback can improve both recall and precision. But, in practice, it has been shown to be most useful for increasing recall in situations where recall is important. 
- In Rocchio (1971) algorithm, $\alpha, \beta, \gamma$ controls the balance between trusting the judged document set versus the query: If we have a lot of judged documents, we would like a higher $\beta$ and $\gamma$. 
- Relevance feedback can improve both recall and precision. But, in practice, it has been shown to be most useful for increasing recall in situations where recall is important.
- In fact, many systems, such as the image search system, allow only positive feedback, which is equivalent to setting $\gamma = 0$. Another alternative is to use only the marked nonrelevant document that received the highest ranking from the IR system as negative feedback (here, $|D_{nr}| = 1$ in Equation (1)). 
- Some experimental results have also suggested that using a limited number of terms like this may give better results (Harman 1992), although other work has suggested that using more terms is better in terms of retrieved document quality (Buckley et al. 1994). But, the long queries may result in a high computing cost for the retrieval and potentially long response times for the user. 
- In general, RF has been little used in web searches.
- Pseudo-relevance feedback mostly works. Evidence suggests that it tends to work better than global analysis. It has been found to improve performance in the TREC ad hoc task.
- Implicit feedback is less reliable than explicit feedback but is more useful than pseudo RF, which contains no evidence of user judgments.
- Use of query expansion generally increases recall and is widely used in many science and engineering fields. 
- Simply using word cooccurrence is more robust (it cannot be misled by parser errors) for automatic thesaurus generation, but using grammatical relations is more accurate.
- Query expansion is often effective in increasing recall. However, query expansion may also significantly decrease precision, particularly when the query contains ambiguous terms.
- Overall, query expansion is less successful than RF, although it may be as good as pseudo RF.
