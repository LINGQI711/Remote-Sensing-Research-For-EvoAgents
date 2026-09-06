# Experience-Driven Multi-Agent Systems Are Training-free Context-aware Earth Observers

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/arXiv/Experience-Driven%20Multi-Agent%20Systems%20Are%20Training-free%20Context-aware%20Earth%20Observers.pdf) · [Source version](https://arxiv.org/abs/2602.02559v1)

**Venue:** arXiv preprint

**Version read:** v1

**Topic:** Experience-driven exploration and memory

## 1. What problem does it address?

Frozen agents repeatedly make context-dependent tool and parameter errors, and storing raw trajectories does not reliably turn failures into reusable guidance.

## 2. How does it solve the problem?

A retrieval-augmented orchestrator decomposes tasks, explores alternative tool parameters through multiple agents, and contrasts successful and failed attempts. Root-cause analysis distills experience into contextual tool constraints for subsequent retrieval, without updating language-model weights.

## 3. What experiments were conducted?

- Evaluates on ThinkGeo, an Earth-Agent task set, and GeoPlan, comparing experience and workflow baselines such as ExpeL and AFlow.
- Ablates self-contrast, exploration, and memory components and studies exploration and retrieval settings. The sequential ablation uses a 65-task subset.

## 4. What are the conclusions?

Structured failure analysis and retrieved constraints improve execution in the evaluated settings. On the ablation subset, removing self-contrast reduces the reported score from 76.56 to 54.69. This subset result should not be presented as a full-benchmark score. The method is particularly relevant to training-free experience reuse in remote sensing.

**Reading pointers:** Sections 3–4; PDF pages 3–8.
