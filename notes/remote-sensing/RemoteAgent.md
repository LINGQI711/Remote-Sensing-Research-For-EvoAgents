# RemoteAgent: Bridging Vague Human Intents and Earth Observation with RL-based Agentic MLLMs

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/arXiv/RemoteAgent%20-%20Bridging%20Vague%20Human%20Intents%20and%20Earth%20Observation%20with%20RL-based%20Agentic%20MLLMs.pdf) · [Source version](https://arxiv.org/abs/2604.07765v2)

**Venue:** arXiv preprint

**Version read:** v2

**Topic:** Resolving vague intents with reinforcement learning

## 1. What problem does it address?

Users often describe an Earth observation need vaguely instead of supplying a precise task label, output format, and tool specification.

## 2. How does it solve the problem?

VagueEO supplies ambiguous requests, and reinforcement learning with GRPO and LoRA adapts Qwen2.5-VL-7B to infer intent and choose execution strategies. Sparse visual tasks can be handled internally, while dense predictions use specialized tools through MCP.

## 3. What experiments were conducted?

- Measures intent understanding and evaluates grounding on DIOR-RSVG, reasoning on EarthReason, and counting on HRRSD and DOTA-v2.
- Tests detection on DIOR and DIOR-R and segmentation on iSAID and Potsdam, alongside comparisons and component studies.

## 4. What are the conclusions?

Intent-aware training supports a broad interface to remote sensing tasks, with 95% mean intent accuracy reported. Performance is not best on every downstream benchmark: other methods lead on EarthReason reasoning and HRRSD counting. Dense-task scores reflect the combined agent and external perception tools, not solely the language model.

**Reading pointers:** Method and experimental sections; PDF pages 3–8.
