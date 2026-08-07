---
layout: post
title: "Lexical Reranking of Semantic Retrieval (LeSeR) for Regulatory QA"
date: 2025-04-15 00:00:00 +0000
image: /images/leser.png  # optional thumbnail, update or remove if unused
categories: [research]
authors: "Jebish Purbey, <strong>Drishti Sharma</strong>, Siddhant Gupta, Khawaja Murad, Siddartha Pullakhandam, Ram Mohan Rao Kadiyala"
venue: "COLING 2025 (RegNLP Track, 4th Place)"
link: https://arxiv.org/pdf/2412.06009  # replace with actual paper link
arxiv: https://aclanthology.org/2025.regnlp-1.6.pdf
excerpt: "This work introduces LeSeR (Lexical Reranking of Semantic Retrieval), a hybrid retrieval approach that combines dense semantic retrieval, using fine-tuned embedding models on query-passage pairs, with a second-stage reranking via BM25, a classical lexical retrieval method. This decoupled two-stage pipeline enhances both recall and precision, outperforming standalone dense or lexical methods. Multiple embedding models, including Stella, BGE, CDE, and MPNet, were fine-tuned using Multiple Negative Symmetric Ranking (MNSR) Loss, with BGE_MNSR integrated into LeSeR (BGE_LeSeR) yielding the best retrieval performance, achieving Recall@10 of 0.8201 and mAP@10 of 0.6655. For answer generation, the optimal combination was BGE_LeSeR paired with Qwen2.5 7B, attaining the highest RePASs score of 0.4340, reflecting strong performance in entailment, obligation coverage, and minimal contradiction."
---

This work introduces **LeSeR** (Lexical Reranking of Semantic Retrieval), a hybrid method that first performs dense semantic retrieval using fine-tuned embedding models on query-passage pairs, and then reranks the results using BM25, a classical lexical retrieval algorithm.

This two-stage decoupled pipeline improves both recall and precision, outperforming standalone dense or lexical methods.

We evaluated multiple embedding models, including **Stella**, **BGE**, **CDE**, and **MPNet**, with fine-tuning using **Multiple Negative Symmetric Ranking (MNSR)** Loss. Among these, **BGE_MNSR integrated with LeSeR (BGE_LeSeR)** achieved the best retrieval performance:

- **Recall@10**: 0.8201  
- **mAP@10**: 0.6655  

For answer generation, the best combination was **BGE_LeSeR + Qwen2.5 7B**, achieving the highest **RePASs score (0.4340)**, demonstrating strong entailment, obligation coverage, and minimal contradiction.
