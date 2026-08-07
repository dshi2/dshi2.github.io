---
layout: post
title: "Detection of Language, Hate Speech, and Targets using LLMs in Devanagari Script"
date: 2025-01-15 00:00:00 +0000
image: /images/devanagari-hatespeech.png  # optional image
categories: [research]
authors: "Jebish Purbey, Siddartha Pullakhandam, Kanwal Mehreen, Muhammad Arham, <strong>Drishti Sharma</strong>, Ashay Srivastava, Ram Mohan Rao Kadiyala"
venue: "COLING 2025 (CHiPSAL Track)"
link: https://arxiv.org/pdf/2411.06850  # replace with actual link
arxiv: https://aclanthology.org/2025.chipsal-1.23.pdf
excerpt: "This work presents a modular multilingual NLP system tailored for five Devanagari-script languages: Hindi, Nepali, Marathi, Sanskrit, and Bhojpuri, targeting three key tasks: language identification, hate speech detection, and hate speech target classification. Each task is addressed with distinct models and strategies: language identification uses an ensemble of fine-tuned IndicBERT V2, MuRIL, and Gemma-2 9B models, achieving high accuracy through majority voting with fallback logic; hate speech detection employs another ensemble combining IndicBERT V2, Gemma-2 9B, and Gemma-2-27B, all fine-tuned using ORPO, with BERT-based models further enhanced by focal loss to handle severe class imbalance; and target classification achieves its best performance using a single Gemma-2 27B model fine-tuned with ORPO, without relying on ensembling. The system achieves F1 scores of 0.9980 for language identification, 0.7652 for hate speech detection, and 0.6804 for target classification."
---

This work presents a modular multilingual NLP system for five Devanagari-script languages: **Hindi, Nepali, Marathi, Sanskrit, and Bhojpuri**, designed to tackle three tasks:

1. **Language identification**  
2. **Hate speech detection**  
3. **Hate speech target classification**

Each task is addressed using a distinct set of models and strategies:

- **Language Identification**: An ensemble of fine-tuned IndicBERT V2, MuRIL, and Gemma-2 9B models achieves high accuracy via majority voting with fallback logic.

- **Hate Speech Detection**: Another ensemble combines IndicBERT V2, Gemma-2 9B, and Gemma-2 27B, all fine-tuned using **Odds Ratio Preference Optimization (ORPO)**. BERT-based models also use **focal loss** (α = 0.35, γ = 4.0) to counter severe class imbalance.

- **Target Classification**: The best result was achieved by a single Gemma-2 27B model fine-tuned with ORPO, without ensembling.

All decoder-only models were trained using **4-bit LoRA** for memory-efficient optimization.

### Results

- **Sub-task A (Lang ID)**: F1 = 0.9980  
- **Sub-task B (Hate Detection)**: F1 = 0.7652  
- **Sub-task C (Target Classification)**: F1 = 0.6804  

These results demonstrate the effectiveness of task-specific, resource-conscious LLM design for low-resource, script-sensitive language processing.



This work presents a modular multilingual NLP system tailored for five Devanagari-script languages: Hindi, Nepali, Marathi, Sanskrit, and Bhojpuri, targeting three key tasks: language identification, hate speech detection, and hate speech target classification. Each task is addressed with distinct models and strategies: language identification uses an ensemble of fine-tuned IndicBERT V2, MuRIL, and Gemma-2 9B models, achieving high accuracy through majority voting with fallback logic; hate speech detection employs another ensemble combining IndicBERT V2, Gemma-2 9B, and Gemma-2 27B, all fine-tuned using Odds Ratio Preference Optimization (ORPO), with BERT-based models further enhanced by focal loss (α = 0.35, γ = 4.0) to handle severe class imbalance; and target classification achieves its best performance using a single Gemma-2 27B model fine-tuned with ORPO, without relying on ensembling. All decoder-only models were optimized using 4-bit LoRA for memory efficiency. The system achieves strong results across tasks, with F1 scores of 0.9980 for language identification, 0.7652 for hate speech detection, and 0.6804 for target classification, highlighting the effectiveness of task-specific, resource-conscious LLM design in low-resource, script-sensitive language contexts.
