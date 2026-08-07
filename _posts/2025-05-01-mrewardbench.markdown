---
layout: post
title: "M-REWARDBENCH: Evaluating Reward Models in Multilingual Settings"
date: 2025-06-15 00:00:00 +0000
image: /images/mrewardbench.png  # optional thumbnail image
categories: research
author: "Drishti Sharma"
authors: "Srishti Gureja, Lester James V. Miranda, Shayekh Bin Islam, Rishabh Maheshwary, <strong>Drishti Sharma</strong>, Gusti Winata, Nathan Lambert, Sebastian Ruder, Sara Hooker, Marzieh Fadaee"
venue: "ACL 2025 (Main Conference)"
advisors: "Nathan Lambert, Sebastian Ruder, Sara Hooker, Marzieh Fadaee"
link: https://arxiv.org/pdf/2410.15522  # replace with actual link
arxiv: https://arxiv.org/pdf/2410.15522
code: https://github.com/Cohere-Labs-Community/m-rewardbench  # replace with actual repo
dataset: https://huggingface.co/datasets/CohereLabsCommunity/multilingual-reward-bench  # replace with dataset
leaderboard: https://coherelabscommunity-m-rewardbench.hf.space/  # replace if available
excerpt: "This work introduces M-REWARDBENCH, the first large-scale benchmark for evaluating reward models (RMs) in multilingual settings, encompassing 23 languages across 8 scripts and 5 language families. The benchmark evaluates four key capabilities: chat, safety, reasoning, and translation, using 2.87k human-aligned preference instances. A total of 25 reward models, including Classifier, Generative, and Implicit (DPO-trained) types, are assessed. Results show that Generative RMs, such as GPT-4 Turbo, achieve the highest multilingual performance and cross-lingual consistency, with only a 3% average drop compared to English. In contrast, Classifier and Implicit RMs show greater performance declines (~8-13%) and higher volatility, particularly in subjective domains like chat and safety. RM performance is also influenced by translation quality, language resource availability, and script type."
---

This work presents **M-REWARDBENCH**, the first large-scale benchmark for evaluating reward models (RMs) in multilingual settings, covering 23 languages across 8 scripts and 5 language families.

The benchmark assesses four core capabilities:

1. Chat  
2. Safety  
3. Reasoning  
4. Translation  

using 2.87k human-aligned preference instances.

A total of 25 reward models, spanning Classifier, Generative, and Implicit (DPO-trained) types, are evaluated.

### Key findings:

- Generative RMs (e.g., GPT-4 Turbo) achieve the highest multilingual performance and cross-lingual consistency, with only a 3% average performance drop compared to English.
- Classifier and Implicit RMs exhibit larger drops (~8-13%) and greater volatility, especially in subjective categories like chat and safety.
- Translation quality, language resource availability, and script type (e.g., Latin, Cyrillic) significantly impact RM performance.
- For translation, the benchmark incorporates easy and hard subsets from the MAPLE dataset across four directions (en↔zh, en↔de), showing that harder tasks consistently reduce accuracy.
- Performance improves by 1-3% when using higher-quality translations (Google Translate over NLLB-3.3B).
