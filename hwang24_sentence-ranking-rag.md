---
title: DSLR - Sentence Ranking Rag
refs:
    title: >
        DSLR - Document Refinement with Sentence-Level Re-ranking and Reconstruction 
        to Enhance Retrieval-Augmented Generation
    author: Taeho Hwang
    pub_date: 8 Jul 2024
    arxiv: 2407.03627v2 

tags: #llm #rag #ir
---

[Go to paper](https://arxiv.org/abs/2407.03627v2)

## Summary 

It decompose passages into sentece level, then rank them based on the relevancy to the query.
Removing any sentence below the threshold, resulting in variable length passages.
Ranked sentences then rearranged relative to the original position to maintain the context.


## Limitation

- Removing senteces below threshold, creating a risk of unintentionally removing 
sentences that might be relevant to the query.

- Still suffer from bad/incorrect sparse retrieval result,
added with sentence removal, the info provided to LLM is even smaller.


## Key points
 - Doesn't require pretraining
 - Relatively simple and easy to implement
 - Currently using off the shelf algorithm/method


## Result
