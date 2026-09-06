# Earth-Agent: Unlocking the Full Landscape of Earth Observation with Agents

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/ICLR/Earth-Agent%20-%20Unlocking%20the%20Full%20Landscape%20of%20Earth%20Observation%20with%20Agents.pdf) · [Source version](https://arxiv.org/abs/2509.23141v3)

**Venue:** ICLR 2026

**Version read:** v3

**Topic:** Multimodal Earth observation tools and evaluation

## 1. What problem does it address?

Earth observation agents often cover only RGB imagery or a narrow set of tools, leaving spectral data, derived products, and professional quantitative analysis underexplored.

## 2. How does it solve the problem?

Earth-Agent exposes 104 professional tools through MCP and connects reasoning to RGB imagery, spectral observations, and Earth products. EarthBench evaluates both autonomous planning and execution from explicit instructions, with step-level and final-outcome measures.

## 3. What experiments were conducted?

- Evaluates 14 representative task types and 13 language-model backbones, including closed and open models.
- Compares domain models and general agents and analyzes tool selection, parameters, and final answers in autonomous-planning and instruction-following settings.

## 4. What are the conclusions?

Broad tool access makes heterogeneous Earth observation workflows possible, but execution errors remain a major bottleneck. In the version read, GPT-5 scores 65.99 for autonomous planning and 62.35 for instruction following in Table 1: more explicit instructions do not automatically improve the final result. Its benchmark and toolkit provide infrastructure for studying agents, rather than proving lifelong self-improvement.

**Reading pointers:** Sections 3–5; Table 1; PDF pages 4–10.
