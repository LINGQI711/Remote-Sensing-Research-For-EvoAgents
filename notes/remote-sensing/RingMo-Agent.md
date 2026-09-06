# RingMo-Agent: A Unified Remote Sensing Foundation Model for Multi-Platform and Multi-Modal Reasoning

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2025/arXiv/RingMo-Agent%20-%20A%20Unified%20Remote%20Sensing%20Foundation%20Model%20for%20Multi-Platform%20and%20Multi-Modal%20Reasoning.pdf) · [Source version](https://arxiv.org/abs/2507.20776v2)

**Venue:** arXiv preprint 2025

**Version read:** v2

**Topic:** Multi-platform, multi-modal remote sensing foundation models

## 1. What problem does it address?

Remote sensing inputs vary across satellite/UAV platforms and optical, SAR, and infrared sensors. Models trained mainly on homogeneous imagery struggle to unify fine-grained perception and longer spatial reasoning tasks.

## 2. How does it solve the problem?

Build RS-VL3M with over three million image–text pairs, use modality-specific embedding layers, and represent tasks through dedicated tokens. A trajectory decoder handles sequential spatial outputs. Training proceeds through vision–language generation and instruction tuning, with task-specific fine-tuning reported separately from zero-shot evaluation.

## 3. What experiments were conducted?

- Reasoning tasks include CityNav navigation/task scheduling, SkyAgent-Plan3k action decisions, FIT-RS and ReCon1M-REL relation reasoning, and ReCon1M-DEC instruction decomposition.
- Perception evaluation covers captioning, VQA, classification, and detection, including RSVQA-LR, UCM, SARDet-100k, and infrared datasets.
- Metrics include navigation error/success/SPL, BLEU/SPICE, F1, accuracy, and mAP@50 as appropriate. Baselines span specialist models, general VLMs, and remote sensing VLMs.
- Ablates two-stage training, modality-specific embeddings, and the trajectory decoder.

## 4. What are the conclusions?

The results support broad remote-sensing specialization: relation F1 reaches 75.34 on FIT-RS and 90.23 on ReCon1M-REL; SARDet-100k mAP@50 reaches 53.84. However, comparisons often mix fine-tuned and zero-shot systems. CityNav test-unseen success remains 4.74%, below AerialVLN+GSM at 6.72%. This paper is chiefly a trained foundation-model reference, not evidence of continual external skill evolution.

**Reading pointers:** Section 5; Tables 3–6 and 16–20; PDF pages 11–18.
