# Voyager: An Open-Ended Embodied Agent with Large Language Models

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/general-skills/2024/TMLR/Voyager%20-%20An%20Open-Ended%20Embodied%20Agent%20with%20Large%20Language%20Models.pdf) · [Source version](https://arxiv.org/abs/2305.16291v2)

**Venue:** Transactions on Machine Learning Research

**Version read:** v2

**Topic:** Executable skill libraries and automatic curricula

## 1. What problem does it address?

Embodied agents need to discover new objectives and retain useful behaviors instead of repeatedly solving each task from scratch.

## 2. How does it solve the problem?

An automatic curriculum proposes progressively useful Minecraft tasks. GPT-4 generates executable code, repairs it using environment feedback and self-verification, and stores successful programs in a retrievable skill library. Model weights remain fixed.

## 3. What experiments were conducted?

- Tests open-ended Minecraft exploration, unique items, travel, technology-tree progress, and transfer to a new world.
- Compares adapted ReAct, Reflexion, and AutoGPT agents and ablates curriculum, skill memory, and feedback components.

## 4. What are the conclusions?

Executable skills and a curriculum improve exploration and reuse in the evaluated environment. The system operates through high-level Minecraft APIs, so the results should not be read as a raw-pixel, low-level control comparison. The local PDF is arXiv v2; numerical claims from later publication versions may differ.

**Reading pointers:** Sections 2–3; exploration, transfer, and component-ablation results.
