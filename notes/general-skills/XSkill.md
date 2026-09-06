# XSkill: Continual Learning from Experience and Skills in Multimodal Agents

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/general-skills/2026/ICML/XSkill%20-%20Continual%20Learning%20from%20Experience%20and%20Skills%20in%20Multimodal%20Agents.pdf) · [Source version](https://arxiv.org/abs/2603.12056v2)

**Venue:** ICML 2026 (accepted)

**Version read:** v2

**Topic:** Continual learning from experiences and skills

## 1. What problem does it address?

Multimodal agents repeatedly rediscover procedures, make tool-use mistakes, and struggle to adapt fixed workflows to a new visual context. Existing experience memories often underuse visual evidence.

## 2. How does it solve the problem?

An accumulation phase summarizes multiple rollouts with visual grounding and cross-rollout critique. Separate managers consolidate reusable skill documents and tactical experience entries. At inference time, task decomposition, retrieval, and adaptation provide guidance matched to the current task and visual state. Skills encode procedures; experiences guide context-dependent decisions.

## 3. What experiments were conducted?

- Main evaluation: VisualToolBench, TIR-Bench, MMSearch-Plus, and AgentVista, with 100 tasks per benchmark reserved for knowledge accumulation and the remainder used for evaluation.
- Four backbones: Gemini-2.5-Pro, Gemini-3-Flash, GPT-5-mini, and o4-mini. Baselines include no tools, tools only, AWM, Dynamic CheatSheet, and Agent-KB; metrics are Average@4 and Pass@4.
- Ablates experiences, skills, both knowledge managers, task decomposition, and adaptation; analyzes execution errors, tool distributions, and accumulation rollout counts.
- Zero-shot transfer uses VisualToolBench knowledge on TIR-Bench and MMSearch-Plus knowledge on MMBrowseComp.

## 4. What are the conclusions?

Average@4 improves by 2.58–6.71 points over tools-only baselines across backbone averages. Skills reduce execution mistakes, while experiences change tool selection toward task-relevant strategies. Crucially, the conclusion explicitly describes the evaluated setting as one accumulation-then-test cycle; repeated lifelong improvement is an architectural possibility rather than a demonstrated long-term result.

**Reading pointers:** Sections 3 and 5; Tables 2–4 and Figures 3–5; PDF pages 5–9.
