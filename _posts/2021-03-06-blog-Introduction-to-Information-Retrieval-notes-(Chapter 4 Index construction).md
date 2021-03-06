---
title: 'Introduction to Information Retrieval Notes (Chapter 4 Index construction)'
date: 2021-03-06
permalink: /posts/2021/03/blog-Information-Retrieval-Notes-Chapter-04/
tags:
  - Information Retrieval
  - Map Reduce
  - Index Construction
---

You can click [**here**](https://pridelee.github.io/files/blog/Chapter-4-Index-Constriction.pdf) and [**here**](https://zhuanlan.zhihu.com/p/354656012) to read full blog.

**Summary**

- The design of indexing algorithms is governed by hardware constraints. 
- Blocked sort-based indexing, an efficient single-machine algorithm designed for static collections that can be viewed as a more scalable version of the basic sort-based indexing algorithm.
- Single-pass in-memory indexing, an algorithm that has even better scaling properties because it does not hold the vocabulary in memory.  
- For very large collections like the web, indexing has to be distributed over computer clusters with hundreds or thousands of machines.
- Collections with frequent changes require dynamic indexing so that changes in the collection are immediately reflected in the index.
- Access to data in memory is much faster than access to data on disk. It takes a few clock cycles (perhaps $5 \times 10^{−9}$ seconds) to access a byte in memory but much longer to transfer it from disk (about $2 \times 10^{−8}$ seconds). Therefore, the data which be accessed frequently should be store in memory.
- When doing a disk read or write, it takes a while for the disk head to move to the part of the disk where the data are located. This time is called the seek time, and it averages 5 ms for typical disks. No data are being transferred during the seek. To maximize data transfer rates, chunks of data that will be read together should therefore be stored contiguously on disk.
- Operating systems generally read and write entire blocks. Thus, reading a single byte from disk can take as much time as reading the entire block. Block sizes of 8, 16, 32, and 64 kilobytes (KB) are common. We call the part of main memory where a block being read or written is stored a buffer.
- Data transfers from disk to memory are handled by the system bus, not by the processor. This means that the processor is available to process data during disk I/O. We can exploit this fact to speed up data transfers by storing compressed data on disk. 
- The blocked sort-based indexing algorithm or BSBI includes four steps: (i) segments the collection into parts of equal size, (ii) sorts the termID–docID pairs of each part in memory, (iii) stores intermediate sorted results on disk, and (iv) merges all intermediate results into the final index.
- The time complexity of BSBI is $O(TlogT)$ because the step with the highest time complexity is sorting, and $T$ is an upper bound for the number of items we must sort (i.e., the number of termID–docID pairs). But the actual indexing time is usually dominated by the time it takes to parse the documents (ParseNextBlock) and to do the final merge (MergeBlocks).
