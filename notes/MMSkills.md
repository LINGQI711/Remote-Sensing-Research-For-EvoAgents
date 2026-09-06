# MMSkills: Towards Multimodal Skills for General Visual Agents

[Library](../README.md) · [All notes](README.md) · [PDF](../papers/2026/arXiv/MMSkills%20-%20Towards%20Multimodal%20Skills%20for%20General%20Visual%20Agents.pdf) · [Source version](https://arxiv.org/abs/2605.13527v3)

**Venue:** arXiv preprint 2026  
**Version read:** v3  
**Topic:** Multimodal skill representation and runtime consultation

## 1. What problem does it address?

Text-only skills describe what to do but may not tell a visual agent whether the current screen matches the right state. Full demonstrations are bulky, while loading many screenshots can distract the main agent.

## 2. How does it solve the problem?

Represent each skill with a descriptor, textual procedure, runtime state cards, and aligned visual keyframes. A generator derives packages from non-test public trajectories. The main agent can consult a temporary branch that selects views, checks applicability, and returns a subgoal, plan, constraints, and verification guidance; actions remain grounded in the live observation.

## 3. What experiments were conducted?

- Evaluates OSWorld, macOSWorld, VAB-Minecraft, and Super Mario Bros from LMGame-Bench across multiple multimodal model families.
- Compares no skills, text-only skills, and MMSkills; reports GUI success, Minecraft success/score, and Mario performance/reward.
- Ablates state cards, images, direct versus branch loading, and view selection. Analyzes invocation frequency, trajectory length, selected views, and action patterns.

## 4. What are the conclusions?

On OSWorld, Gemini 3 Flash rises from 36.65% to 47.97%, and Qwen3-VL-235B from 21.34% to 39.17%. State cards, images, and selective branch consultation each matter. Benefits depend on the setting: Qwen3-VL-8B remains at 6.29% on macOSWorld, and GLM-5V ties text-only skills there. This is a useful skill-design reference; remote-sensing transfer is not evaluated in the paper.

**Reading pointers:** Section 3; Tables 1–3 and Figure 3; PDF pages 6–8. Page numbers refer to the archived PDF. Results are reported by the paper, not independently reproduced.
