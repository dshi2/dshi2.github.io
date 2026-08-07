---
layout: post
title: "Sequential Learning for Claim Verification and Explanation in Financial Domains"
date: 2025-01-10 00:00:00 +0000
image: /images/seqwen.png  # optional thumbnail
categories: research
authors: "Jebish Purbey, Siddhant Gupta, Nikhil Manali, Siddartha Pullakhandam, <strong>Drishti Sharma</strong>, Ashay Srivastava, Ram Mohan Rao Kadiyala"
venue: "COLING 2025 (FINLP Track, 3rd Place)"
arxiv: https://aclanthology.org/2025.finnlp-1.35.pdf  # replace with actual paper or arXiv link
excerpt: "This work presents SeQwen, a sequential learning-based system, which focused on two tasks: classifying financial claims as True, False, or Not Enough Information (NEI), and generating coherent natural language explanations for these classifications. Using the FIN-FACT dataset, the team evaluated several open-source LLMs, including Qwen2.5, Mistral, Llama3, Gemma-2, and Phi-3. SeQwen employed a two-stage sequential fine-tuning strategy: first fine-tuning for claim classification, followed by joint fine-tuning for classification and explanation generation. This approach consistently outperformed single-stage joint training, with Qwen2.5-7B emerging as the top-performing model. The two-stage method led to a 7.1% improvement in overall score and significantly enhanced explanation quality, while merely increasing joint training epochs offered only marginal gains, underscoring the value of sequential fine-tuning."
---

This work presents **SeQwen**, a sequential learning-based system developed for the **COLING 2025 Financial Misinformation Detection (FMD)** challenge.

The challenge involved two core tasks:

1. **Classifying financial claims** as *True*, *False*, or *Not Enough Information (NEI)*  
2. **Generating coherent natural language explanations** for the classification

We used the **FIN-FACT** dataset and evaluated several open-source LLMs, including:

- **Qwen2.5**  
- **Mistral**  
- **Llama3**  
- **Gemma-2**  
- **Phi-3**

Our system used a **two-stage sequential fine-tuning approach**:

- Stage 1: fine-tune for claim classification  
- Stage 2: fine-tune jointly for classification + explanation generation

### Key findings:

- **Qwen2.5 7B** was the best-performing model overall.
- Sequential fine-tuning consistently outperformed single-stage joint training.
- The approach yielded a **7.1% improvement** in overall score and significantly better explanation quality.
- Simply increasing joint training epochs provided only marginal gains compared to the structured two-stage approach.
