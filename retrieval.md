---
title: Retrieval Method 
---

## Sparse Retrieval

Care more about the syntax of documents/collections of data,
The method work on syntax similarity, frequency, or rule based 

+ Fast, efficient, low computing power
+ Doesn't need training
+ Algorithm are easier to reason
- Low accuracy 
- Not capturing synonym or paraphrased text. 


### Etymology

Imagine a single word query on thousands lines of document,
the matching result is a scattered along these documents,
most of them didn't match, empty spaces.


## Dense Retrieval

Capturing semantic, understand the meaning of the documents.
It represented in a high dimensional space, like word embedding.
Basically a job for an LLM.

+ High accuracy
+ Better at handling complex queries
- Black magic, the reasoning behind the retrievals hard to be explained
- Need training
- Computationally expensive 


### Etymology

The name came from how tightly packed (dense) are the vector representing 
the semantic relationship of the word/sentence/documents.
