# MemSkill: Learning and Evolving Memory Skills for Self-Evolving Agents

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/general-skills/2026/arXiv/MemSkill%20-%20Learning%20and%20Evolving%20Memory%20Skills%20for%20Self-Evolving%20Agents.pdf) · [Source version](https://arxiv.org/abs/2602.02474v2)

**Venue:** arXiv preprint

**Version read:** v2

**Topic:** Learning and evolving memory operations

## 1. What problem does it address?

Fixed memory operations may be unsuitable for different tasks, while ad hoc memory writing lacks a learned strategy for choosing how to update memory.

## 2. How does it solve the problem?

A controller selects memory skills, an executor applies them, and a designer refines or adds skills using difficult cases. The controller is optimized with reinforcement learning, while the skill inventory can evolve through language-based design.

## 3. What experiments were conducted?

- Evaluates conversational memory on LoCoMo and LongMemEval, interactive task success and steps on ALFWorld, and transfer to HotpotQA.
- Ablates the controller, designer, random skill selection, fixed primitive operations, and refinement without new-skill creation.

## 4. What are the conclusions?

The experiments support adapting both memory selection and memory operations to the task. Unlike purely inference-time skill-editing systems, MemSkill includes reinforcement learning of its controller and should not be labeled entirely training-free. Memory-question answering and interactive-agent performance are distinct outcomes.

**Reading pointers:** Controller, executor, and designer descriptions; main experiments and ablations.
