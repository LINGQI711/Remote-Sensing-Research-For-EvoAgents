# GeoX: Mastering Geospatial Reasoning Through Self-Play and Verifiable Rewards

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/arXiv/GeoX%20-%20Mastering%20Geospatial%20Reasoning%20Through%20Self-Play%20and%20Verifiable%20Rewards.pdf) · [Source version](https://arxiv.org/abs/2605.20006v1)

**Venue:** arXiv preprint 2026

**Version read:** v1

**Topic:** Self-play training for program-verifiable geospatial reasoning

## 1. What problem does it address?

Questions over area, distance, adjacency, direction, and object relations grow combinatorially with scene complexity. Human-curated remote-sensing QA datasets cover only a small portion of this space. Unverified self-generated data can expand coverage, but noisy questions and answers can accumulate during training.

## 2. How does it solve the problem?

GeoX uses one multimodal policy in two roles: a proposer creates image-conditioned spatial problems as executable programs, and a solver answers them. The shared execution interface combines 22 geometric, topological, and aggregation primitives with the SegEarth-OV3 open-vocabulary segmentation tool. Masking the arguments, output, or program creates abduction, deduction, and induction tasks. Program execution supplies solver rewards, while the proposer receives the highest reward for problems near the solver's current capability boundary. Intermediate execution values remain hidden from the policy to reduce answer-copying shortcuts.

## 3. What experiments were conducted?

- Training uses images from SAMRS-FAST and Globe230k without their human labels.
- VQA evaluation uses RSVQA-HR, EarthVQA, and 17 spatial tasks from GEOBench-VLM; counting evaluation uses HRRSD and RSOD.
- Qwen2.5-VL-7B-Instruct and LLaVA-1.5-7B are evaluated as base policies and compared with remote-sensing VLMs trained on curated data.
- Ablations remove individual reasoning modes, replace adaptive self-play proposals with base-model proposals, or remove the proposer learning signal.

## 4. What are the conclusions?

GeoX improves the three-benchmark VQA average by 5.5 points for LLaVA and 1.9 points for Qwen. Gains concentrate on capabilities that the execution interface can verify, including area, counting, and spatial relations. Results are not uniformly positive: event detection declines for both backbones on GEOBench-VLM, and Qwen's RSOD counting MAE worsens from 3.31 to 3.69. The current verifier depends on one segmentation tool and single-time spatial primitives, so perception errors become reward noise and temporal or metadata reasoning remains outside scope. This is parameter-updating self-play training, not a memory- or skill-evolving agent.

**Reading pointers:** Sections 2-5; Tables 1-4 and 7; Figures 1-5 and 7; PDF pages 3-14 and appendices.
