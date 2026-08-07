---
layout: post
title: "Sparse Upcycling VLMs: Efficient Multilingual Adaptation from Dense Models"
date: 2025-04-01 00:00:00 +0000
image: /images/sparse-upcycling.png  # optional
categories: other
rank: 3
author: "Drishti Sharma"
authors: "Mayank, Trishanu, Alvin, Ahmad, Shivam, <strong>Drishti</strong>, Alper, Shayekh"
link: https://docs.google.com/presentation/d/1nBIqb9M-Oa5zlDJ3op1MR8vBBUw5-k6YMO6j66cKJgQ/edit?slide=id.g146d9451f85_1_445#slide=id.g146d9451f85_1_445
slides: https://docs.google.com/presentation/d/1nBIqb9M-Oa5zlDJ3op1MR8vBBUw5-k6YMO6j66cKJgQ/edit?slide=id.g146d9451f85_1_445#slide=id.g146d9451f85_1_445
excerpt: "This project explores sparse upcycling of dense vision-language models (VLMs) as an efficient strategy for multilingual adaptation. Using a parameter-efficient framework, the approach injects lightweight routing into pretrained dense architectures, upcycling both vision encoders and decoder FFNs, without modifying the vision tower. Evaluated on a multilingual dataset of 1.58M samples across 10 languages and 3 domains, the study compares decoder-only, encoder+decoder, and reciprocal upcycling. Results show upcycled small models achieving up to 47.1% win rate against Qwen2-VL-2B with no vision modifications, and demonstrate that decoder-side adaptation drives most of the language lift, while reciprocal tuning improves vision-language alignment."
---
