---
layout: post
title: "Behind Maya: Building a Multilingual Vision Language Model"
date: 2025-06-10 00:00:00 +0000
image: /images/maya.png  # optional, update or remove
categories: research
author: "Drishti Sharma"
authors: "Nahid Alam, Karthik Reddy Kanjula, Surya Guthikonda, Timothy Chung, Bala Krishna S Vegesna, Abhipsha Das, Anthony Susevski, Ryan Sze-Yin Chan, S M Iftekhar Uddin, Shayekh Bin Islam, Roshan Santhosh, Snegha A, <strong>Drishti Sharma</strong>, Chen Liu, Isha Chaturvedi, Genta Indra Winata, Ashvanth.S, Snehanshu Mukherjee, Alham Fikri Aji"
venue: "VLMs4ALL Workshop @ CVPR 2025"
link: https://arxiv.org/pdf/2505.08910  # replace with actual paper link
code: https://github.com/nahidalam/maya  # optional
arxiv: https://arxiv.org/pdf/2505.08910
excerpt: "This work introduces Maya, an open-source multilingual VLM designed to improve performance in low-resource languages and culturally diverse contexts where existing VLMs often underperform. Maya is built on two key contributions: a multilingual image-text pretraining dataset comprising 4.4 million samples across eight languages, English, Chinese, French, Spanish, Russian, Hindi, Japanese, and Arabic, generated using a hybrid translation framework that integrates Aya 35B, BLEU/N-gram scoring, and balanced sampling from the LLaVA dataset; and a multilingual multimodal architecture that replaces CLIP with SigLIP as the vision encoder for better multilingual adaptability and variable patch size support, while using Aya-23 8B as the LLM, which supports 23 languages and an 8K context window. Visual features are aligned with language space via a 2-layer MLP with GELU activation, following techniques from LLaVA 1.5. Maya outperforms PALO-7B on LLaVA-Bench-In-The-Wild.
"
---

This work introduces **Maya**, an open-source multilingual vision-language model (VLM) designed to address the underperformance of existing VLMs in low-resource languages and diverse cultural contexts.

Maya is built on two major contributions:

1. A multilingual image-text pretraining dataset with **4.4M samples** across 8 languages: English, Chinese, French, Spanish, Russian, Hindi, Japanese, and Arabic, created using a hybrid translation framework that combines Aya 35B, BLEU/N-gram scoring, and balanced sampling from the LLaVA dataset.

2. A multilingual multimodal model architecture using **SigLIP** as the vision encoder (replacing CLIP for multilingual adaptability and variable patch size support) and **Aya-23 8B** as the LLM, which supports 23 languages and an 8K context window.

Visual features are projected through a 2-layer MLP with GELU activation to align with language space, following techniques from LLaVA 1.5.

**Maya outperforms PALO-7B** on LLaVA-Bench-In-The-Wild, offering a strong multilingual alternative to existing VLMs.
