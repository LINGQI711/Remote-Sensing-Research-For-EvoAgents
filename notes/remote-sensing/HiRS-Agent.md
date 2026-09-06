# HiRS-Agent: A Hierarchical Multi-Agent System for Reliable Long-Horizon Remote Sensing Task Solving

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/ACM-MM/HiRS-Agent%20-%20A%20Hierarchical%20Multi-Agent%20System%20for%20Reliable%20Long-Horizon%20Remote%20Sensing%20Task%20Solving.pdf) · [Source version](https://arxiv.org/abs/2608.30672v1)

**Venue:** ACM Multimedia 2026 (accepted)

**Version read:** v1

**Topic:** Hierarchical remote sensing agents and reliable execution

## 1. What problem does it address?

A single controller struggles with multi-stage remote sensing workflows: domain knowledge, tool selection, and intermediate errors become entangled, causing failures to propagate through the pipeline.

## 2. How does it solve the problem?

A Manager handles task decomposition, routing, verification, replanning, and stopping. Specialists cover surface parsing, physical retrieval, and statistical analysis. All roles share one Qwen3 backbone and are distinguished by prompts. Two-stage expert tuning aligns domain knowledge and workflows; verification-guided hierarchical RL uses separate manager-level and specialist-level objectives, implemented with GRPO and LoRA.

## 3. What experiments were conducted?

- Earth-Bench and ThinkGeo evaluate tool selection, execution order, arguments, efficiency, and final answers; Earth-Bench uses Autonomous Planning (AP) and Instruction Following (IF).
- Tests Qwen3-4B and Qwen3-8B, with proprietary/open-source model references and comparisons to generic and remote-sensing agent architectures. Architecture comparisons use a shared trained checkpoint.
- RS-EXPERT-BENCHMARK measures in-domain and out-of-domain expertise; MMLU-Redux, MATH-500, and Multi-IF check general capability retention.
- Ablations remove training stages, verification, and specialist organization to separate their contributions.

## 4. What are the conclusions?

On Earth-Bench, Qwen3-4B final accuracy rises from 15.73/10.08 to 43.95/45.56 in AP/IF. Expertise, hierarchy, and verification contribute complementary gains. The evidence supports improved small-model reliability, not dominance over every larger model: several proprietary baselines retain higher final accuracy. Gains also include parameter training, so this is not a purely training-free evolution method.

**Reading pointers:** Sections 3–4; Tables 1–4; PDF pages 6–8.
