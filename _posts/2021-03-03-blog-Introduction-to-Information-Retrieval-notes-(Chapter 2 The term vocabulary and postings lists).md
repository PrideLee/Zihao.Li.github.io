---
title: 'Introduction to Information Retrieval Notes (Chapter 2 The term vocabulary and postings lists)'
date: 2021-03-03
permalink: /posts/2021/03/blog-Information-Retrieval-Notes-Chapter-02/
tags:
  - Information Retrieval
  - Vocabulary and posting lists
  - Web Search
---

**Summary**

- There is a trade-off for basic/minimum unit design. If the units get too small, we are likely to miss important passages because terms were distributed over several mini-documents, whereas if units are too large, we tend to get spurious matches, and the relevant information is hard for the user to find. Consequently, it is also the dilemma between precision and recall.
- The index granularity is also significant for the IR system. The person who is deploying the system must have a good understanding of the document collection, the users, and their likely information needs and usage patterns. 
- In Chinese, most words are short (the commonest length is two characters).
- The general strategy for determining a stop list is to sort the terms by collection frequency (the total number of times each term appears in the document collection) and then to take the most frequent terms, often hand-filtered for their semantic content relative to the domain of the documents being indexed, as a stop list, the members of which are then discarded during indexing. 
- For keywords search, stop words may be useless, while this is not true for phrase searches.
- Web search engines generally do not use stop lists.
- The most common algorithm for stemming English, and one that has repeatedly been shown to be empirically very effective, is [Porter’s algorithm](www.tartarus.org/˜martin/PorterStemmer/) (Porter 1980). 
- Doing full morphological analysis produces at most very modest benefits for retrieval.
- Although normalization helps a lot for some queries, it equally hurts performance a lot for others.
- Stemming increases recall while harming precision. 
- There is a trade-off between spaced skip and comparisons to skip pointers. More skips mean shorter skip spans and that we are more likely to skip. But it also means lots of comparisons to skip pointers and lots of space storing skip pointers. Fewer skips mean few pointer comparisons, but then long skip spans, which means that there will be fewer opportunities to skip. A simple heuristic for placing skips, which has been found to work well in practice, is that for a postings list of length $P$, use $\sqrt P$ evenly spaced skip pointers.
-  Character bigram indexes are perhaps the most standard approach to indexing Chinese, although some systems use word segmentation. 
- Due to differences in the language and writing system, word segmentation is most usual for Japanese (Luk and Kwok 2002; Kishida et al. 2005). 
- Diacritic removal gains up to 23% (being especially helpful for Finnish, French, and Swedish). 
- Stemming helped markedly for Finnish (30% improvement) and Spanish (10% improvement), but for most languages, including English, the gain from stemming was in the range 0–5%, and results from a lemmatizer were poorer still. Compound splitting gained 25% for Swedish and 15% for German, but only 4% for Dutch.
- Rather than language-particular methods, indexing character k-grams (as we suggested for Chinese) could often give as good or better results: using within-word character four-grams rather than words gave gains of 37% in Finnish, 27% in Swedish, and 20% in German, while even being slightly positive for other languages, such as Dutch, Spanish, and English. Tomlinson (2003) presents broadly similar results.
- Good queries to include in the phrase index are ones known to be common based on recent querying behavior. 
- Uses indexes of biword and positional sorts as well as a partial next word index as a halfway house between the first two strategies. Such a strategy allows a typical mixture of web phrase queries to be completed in one-quarter of the time taken by use of a positional index alone while taking up 26% more space than the use of a positional index alone.
- Suppose the total number of tokens in the document collection $T$, the complexity of a Boolean query is $O(T)$.
- As for large documents, the required space to store the positional posting is two orders of magnitude to store the postings list. 

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-2-The-term-vocabulary-and-postings-lists.pdf) and [**here**](https://zhuanlan.zhihu.com/p/353915529) to read full blog.
