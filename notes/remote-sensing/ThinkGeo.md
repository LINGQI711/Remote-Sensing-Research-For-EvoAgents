# ThinkGeo: Evaluating Tool-Augmented Agents for Remote Sensing Tasks

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2025/arXiv/ThinkGeo%20-%20Evaluating%20Tool-Augmented%20Agents%20for%20Remote%20Sensing%20Tasks.pdf) · [Source version](https://arxiv.org/abs/2505.23752v3)

**Venue:** arXiv preprint

**Version read:** v3

**Topic:** Step-level evaluation of remote sensing tool use

## 1. What problem does it address?

A plausible final explanation can hide incorrect tool choices, arguments, and intermediate reasoning in remote sensing agents.

## 2. How does it solve the problem?

ThinkGeo provides 486 tasks with 1,778 expert-verified reasoning steps across seven application domains. It evaluates a ReAct-style agent using perception, operation, and logic tools, separating instruction, tool, argument, summary, and final-answer quality.

## 3. What experiments were conducted?

- Uses optical and SAR sources, including object detection, land-use, disaster, and other application datasets; the main analysis emphasizes optical tasks.
- Compares language-model backbones under a shared tool framework and reports step-level and final-answer metrics.

## 4. What are the conclusions?

Correct-looking tool use and fluent summaries do not imply task completion. For example, GPT-4o obtains 67.73 tool accuracy but only 34.75 argument accuracy and 9.78 final-answer accuracy in the reported main table. ThinkGeo is useful for diagnosing agent failures and validating later learning methods; it does not itself introduce a trained or self-evolving agent.

**Reading pointers:** Benchmark construction and evaluation sections; PDF pages 3–9; supplementary SAR evaluation.
