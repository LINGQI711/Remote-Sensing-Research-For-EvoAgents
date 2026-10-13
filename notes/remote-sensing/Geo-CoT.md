# Towards Faithful Reasoning in Remote Sensing: A Perceptually-Grounded GeoSpatial Chain-of-Thought for Vision-Language Models

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/ICLR/Towards%20Faithful%20Reasoning%20in%20Remote%20Sensing%20-%20A%20Perceptually-Grounded%20GeoSpatial%20Chain-of-Thought%20for%20Vision-Language%20Models.pdf) · [Source version](https://arxiv.org/abs/2509.22221v2) · [Publication](https://openreview.net/forum?id=lJ7zecny2e) · [Code](https://github.com/minglangL/RSThinker)

**Venue:** ICLR 2026

**Version read:** arXiv v2

**Topic:** Perceptually grounded and auditable remote-sensing reasoning

## 1. What problem does it address?

Remote-sensing VLMs can produce correct-looking answers without exposing which image regions support each claim. Final-answer supervision encourages an opaque pixels-to-text mapping, making hallucinations and intermediate perception errors difficult to localize or audit.

## 2. How does it solve the problem?

Geo-CoT organizes analysis as Planning, iterative Grounding, and Synthesis. Intermediate claims must point to spatial evidence such as bounding boxes. Geo-CoT380k contains 384,591 structured traces across grounding, detection, counting, classification, captioning, and VQA. A two-stage alignment procedure first uses supervised fine-tuning to install the reasoning structure and then applies GRPO with task-specific outcome rewards and a KL constraint. The resulting model, RSThinker, emits both the answer and a spatially grounded analytical trace.

## 3. What experiments were conducted?

- Training combines VRSBench, FIT-RS, NWPU-RESISC45, AID, DIOR-RSVG, DOTA-v2, HRRSD, RSVQA-HR, and several captioning datasets.
- Evaluation covers visual grounding, object detection and counting, scene classification, captioning, and VQA, including zero-shot transfer.
- Baselines include proprietary VLMs, general open VLMs, reasoning-oriented VLMs, and remote-sensing VLMs such as GeoChat, VHM, SkySenseGPT, and EarthDial.
- Ablations compare answer-only SFT, Geo-CoT SFT, and Geo-CoT SFT followed by GRPO, including the effect of the KL constraint.

## 4. What are the conclusions?

RSThinker reports strong results across the evaluated task families. For example, DIOR-RSVG reaches 93.1 Acc@0.5 and 89.02 mIoU, while DOTA-v2 counting reaches 43.93 accuracy with 2.728 MAE. In the main ablation, Geo-CoT SFT plus GRPO raises grounding mIoU from 56.26 for the base model to 89.02 and detection mAP@0.5 from 3.56 to 77.06. The paper also shows an important limitation: a trace can retain the expected syntax while its verification step becomes a stylistic heuristic. Geo-CoT makes such failures more inspectable, but explicit grounding does not by itself prove causal faithfulness. The generated training traces may also inherit GPT-4V style bias.

**Reading pointers:** Sections 3-5; Tables 1 and 4-9; Figures 1-4 and 7; PDF pages 3-12 and appendices.
