---
title: 'Introduction to Information Retrieval (Chapter 10 XML retrieval)'
date: 2021-03-31
permalink: /posts/2021/03/blog-Information-Retrieval-Notes-Chapter-10/
tags:
  - Information Retrieval
  - XML retrieval
  - Structured retrieval
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-10-XML-retrieval.pdf) and [**here**](https://zhuanlan.zhihu.com/p/359519228) to read complete blog.

**Summary**
- There is no consensus yet as to which methods work best for structured retrieval, although many researchers believe that XQuery will become the standard for structured queries.
- Many structured data sources containing text are best modeled as structured documents rather than relational data. 
- Unranked retrieval models like the Boolean model suffer from low recall.
- A perhaps more widespread use of XML is to encode nontext data.
- The data model of parametric and zone search is flat; that is, there is no nesting of attributes. The number of attributes is small. In contrast, XML documents have the more complex tree structure, in which attributes are nested. The number of attributes and nodes is greater than in parametric and zone search.
- For structure retrieval, we can use one of the largest element as the indexing unit, then postprocess search results to the subelement that is the best hit. Unfortunately, this two-stage retrieval process fails to return the best subelement for many queries because the relevance of a whole book is often not a good predictor of the relevance of small subelement within it.  
- Elements that do not meet structural constraints perfectly should be ranked lower, but they should not be omitted from search results.
- The first challenge in structured retrieval is that users want us to return parts of documents (i.e., XML elements), not entire documents as IR systems usually do in unstructured retrieval. 
- A challenge in XML retrieval related to nesting is that we may need to distinguish different contexts of a term when we compute term statistics for ranking, in particular inverse document frequency (idf) statistics.
- In many cases, several different XML schemas occur in a collection because the XML documents in an IR application often come from more than one source. This phenomenon is called schema heterogeneity or schema diversity and presents yet another challenge. 
- Effectiveness in XML retrieval is often lower than in unstructured retrieval because XML retrieval is harder. Instead of just finding a document, we have to find the subpart of a document that is most relevant to the query. 
- Structure helps to increase precision at the top of the results list. 
- Chu-Carroll et al. (2006) also present evidence that XML queries increase precision compared with unstructured queries. 
- Structured retrieval imposes additional constraints on what to return and documents that pass the structural filter are more likely to be relevant. Recall may suffer because some relevant documents will be filtered out, but for precision-oriented tasks structured retrieval is superior.
- There are powerful query languages for XML that can handle numerical attributes, joins, and ordering constraints. The best known of these is XQuery, a language proposed for standardization by the W3C.
- Relational databases are better equipped to handle many structural constraints, particularly joins (but ordering is also difficult in a database framework – the tuples of a relation in the relational calculus are not ordered). For this reason, most data-centric XML retrieval systems are extensions of relational databases. If text fields are short, exact matching meets user needs and retrieval results in form of unordered sets are acceptable, then using a relational database for XML retrieval is appropriate.
- Many other unstructured retrieval methods have been applied to XML retrieval with at least as much success as the vector space model. These methods include language models (cf. Chapter 12; e.g., Kamps et al. (2004), List et al. (2005), Ogilvie and Callan (2005)), systems that use a relational database as a backend (Mihajlovic et al. 2005; Theobald et al. 2005, 2008), probabilistic weighting (Lu et al. 2007), and fusion (Larson 2005).
- There is currently no consensus as to what the best approach to XML retrieval is.
- An active area of XML retrieval research is focused retrieval (Trotman et al. 2007), which aims to avoid returning nested elements that share one or more common subelements.
- Trotman and Geva (2006) argue that XML retrieval is a form of passage retrieval. In passage retrieval (Salton et al. 1993; Hearst and Plaunt 1993; Zobel et al. 1995; Hearst 1997; Kaszkiel and Zobel 1997), the retrieval system returns short passages instead of documents in response to a user query. 
