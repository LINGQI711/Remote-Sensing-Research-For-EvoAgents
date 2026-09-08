# GeoAgent: Learning to Geolocate Everywhere with Reinforced Geographic Characteristics

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/CVPR/GeoAgent%20-%20Learning%20to%20Geolocate%20Everywhere%20with%20Reinforced%20Geographic%20Characteristics.pdf) · [Source version](https://arxiv.org/abs/2602.12617v1) · [Code](https://github.com/HVision-NKU/GeoAgent)

**Venue:** CVPR 2026

**Version read:** arXiv v1

**Topic:** Supporting work: visual geolocation and geographic reasoning

## 1. What problem does it address?

Image geolocation requires interpreting visual clues and expressing locations at different geographic scales. Exact text-match rewards penalize equivalent place names, while automatically generated reasoning traces can reinforce model biases. This work focuses on ground-level imagery, especially street views.

## 2. How does it solve the problem?

GeoSeek provides 10k human-annotated reasoning examples, 20k localization samples, and a roughly 3k-image validation set. Sampling accounts for population, land area, and road mileage. Qwen2.5-VL-7B receives supervised LoRA fine-tuning followed by GRPO reinforcement learning. Spatial distance and hierarchical semantic similarity rewards accommodate alternative place descriptions. A separate consistency agent evaluates whether intermediate reasoning supports location predictions.

## 3. What experiments were conducted?

- Evaluates IM2GPS3K and GeoSeek-Val against conventional geolocation models, general vision-language models, and specialized reasoning models.
- Reports accuracy within 25, 200, 750, and 2,500 km, plus GeoScore on GeoSeek-Val. These are distance thresholds, not exact administrative-boundary accuracy.
- Ablates supervised initialization and the spatial, semantic, and consistency rewards; compares similarity-based rewards with direct text judging.
- Analyzes scene categories, locatability, and qualitative reasoning examples.

## 4. What are the conclusions?

In Table 2, reinforcement learning raises GeoSeek-Val accuracy within 750 km from 47.12% for the supervised model to 60.37%; IM2GPS3K accuracy at that threshold reaches 76.21%. Gains are stronger at broader geographic scales, and the model does not lead every fine-scale metric. Human-like reasoning examples do not establish faithful reasoning in all cases. The work supports geographic reward design and visual geolocation, rather than demonstrating satellite-image analysis or autonomous skill-library evolution.

**Reading pointers:** Sections 3-5; Tables 2-4 and Figures 2-6; PDF pages 4-9. Numerical results refer to the archived arXiv v1.
