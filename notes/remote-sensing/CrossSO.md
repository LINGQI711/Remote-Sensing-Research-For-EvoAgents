# Observe Less, Understand More: Cost-aware Cross-scale Observation for Remote Sensing Understanding

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/ACM-MM/Observe%20Less,%20Understand%20More%20-%20Cost-aware%20Cross-scale%20Observation%20for%20Remote%20Sensing%20Understanding.pdf) · [Source version](https://arxiv.org/abs/2604.11415v2) · [Code](https://github.com/xzhacc/CrossSO)

**Venue:** ACM Multimedia 2026

**Version read:** arXiv v2 camera-ready

**Topic:** Cost-aware selection and completion of cross-scale remote-sensing observations

## 1. What problem does it address?

High-resolution Earth observation provides local detail but is expensive and spatially limited, while low-resolution imagery offers cheap global coverage. Existing sparse high-resolution sampling often scores isolated low-resolution patches and leaves unobserved locations without a task-aligned representation.

## 2. How does it solve the problem?

CrossSO couples an observation policy with latent completion. A sampler combines structural saliency and cross-scale semantic gain to select high-resolution tiles from a global low-resolution overview. An observation-guided predictor places selected high-resolution features back on their grid and uses cross-attention to infer dense task representations at unobserved locations from the low-resolution context. GL-10M supplies nearly 100,000 paired scenes and about 10 million ordered high-resolution tiles for cross-resolution pretraining.

## 3. What experiments were conducted?

- Recognition and retrieval experiments use paired Sentinel-2 and NAIP imagery with seen and unseen OSM concepts.
- Zero-shot transfer is evaluated on EuroSAT, BigEarthNet, and GL-10M.
- Comparisons separate full high-resolution observation, low-resolution-only systems, and sparse-observation methods.
- Metrics jointly report task quality, observed high-resolution budget, multiscale acquisition cost, and inference time. Ablations isolate sampling signals and the latent predictor.

## 4. What are the conclusions?

On the unseen zero-shot retrieval split, CrossSO uses an observed-budget ratio of 0.123 versus 0.236 for the strongest sparse baseline while improving mAP@100 from 0.502 to 0.522 and reducing reported inference time from 233 to 118 seconds. Under the same sampling policy, latent prediction raises the ablation result from 0.475 to 0.522. The method assumes a low-resolution overview, a predefined acquisition grid, and aligned cross-scale training pairs; it does not evaluate temporal revisits, cloud-dependent acquisition, or interactive agent planning. It is included as a supporting observation-policy model rather than as an autonomous agent.

**Reading pointers:** Sections 3-6; Tables 1-4 and Figure 2-3; PDF pages 3-10 and appendices.
