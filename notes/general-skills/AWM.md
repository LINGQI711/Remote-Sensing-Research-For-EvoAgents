# Agent Workflow Memory

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/general-skills/2025/ICML/Agent%20Workflow%20Memory.pdf) · [Source version](https://arxiv.org/abs/2409.07429v1)

**Venue:** ICML 2025

**Version read:** v1

**Topic:** Reusable workflow memory for web agents

## 1. What problem does it address?

Web agents repeatedly reason through recurring interaction patterns and fail to reuse procedures across related tasks.

## 2. How does it solve the problem?

Agent Workflow Memory induces reusable workflows from examples and adds them to the agent context. It supports offline induction from training examples and online induction from successful episodes, allowing later tasks to reuse accumulated procedures.

## 3. What experiments were conducted?

- Evaluates Mind2Web and WebArena, spanning more than 1,000 tasks and 200 websites.
- Studies cross-task, cross-website, and cross-domain settings, compares web-agent baselines, and measures both success and execution steps.

## 4. What are the conclusions?

Workflow memory improves web-task success and can shorten execution. The reported WebArena gain over BrowserGym is 12 percentage points with approximately two fewer steps. Offline and online settings use different evidence sources; online accumulation across evaluation tasks should be considered when comparing protocols.

**Reading pointers:** Workflow induction and experimental sections; Mind2Web and WebArena tables.
