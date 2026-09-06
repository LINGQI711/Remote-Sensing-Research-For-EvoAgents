# RSMeM: Knowledge-Enhanced Memory Evolution for Remote Sensing Agents with Systematic Evaluation

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/ACL/RSMeM%20-%20Knowledge-Enhanced%20Memory%20Evolution%20for%20Remote%20Sensing%20Agents%20with%20Systematic%20Evaluation.pdf) · [Source version](https://arxiv.org/abs/2607.24772v2)

**Venue:** ACL 2026

**Version read:** v2

**Topic:** Knowledge-guided memory evolution

## 1. What problem does it address?

Remote sensing agents need both domain knowledge and reusable failure lessons, but unstructured memories can grow long and retain ineffective execution details.

## 2. How does it solve the problem?

RSMeM combines a hierarchical knowledge base and task cards with failure-aware experience refinement. GeoTraceCompress distills trajectories into compact memories, while reflection records constraints that can guide later tool use.

## 3. What experiments were conducted?

- Evaluates 248 EarthBench tasks with Qwen3-8B, Qwen3-32B, Kimi-K2, and DeepSeek-V3.2, using the professional tool environment with a documented tool substitution.
- Compares Earth-Agent and Reflexion settings and measures execution order, parameters, final accuracy, redundancy, tokens, and experience density.
- Studies repeated attempts: R@3 reruns unresolved cases and retains the latest successful attempt.

## 4. What are the conclusions?

Domain structure and compressed failure lessons improve the evaluated memory pipeline. R@3 is a repeated-attempt setting on the same cases, so its gains should not be interpreted as an isolated transfer test on entirely unseen tasks. Accuracy and memory-efficiency measures should be read together when assessing the benefit of evolution.

**Reading pointers:** Method and experiments; PDF pages 3–9; repeated-attempt evaluation protocol.
