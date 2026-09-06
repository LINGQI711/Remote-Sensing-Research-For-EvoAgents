# Multi-Agent Geospatial Copilots for Remote Sensing Workflows

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2025/IGARSS/Multi-Agent%20Geospatial%20Copilots%20for%20Remote%20Sensing%20Workflows.pdf) · [Source version](https://arxiv.org/abs/2501.16254v1)

**Venue:** IGARSS 2025

**Version read:** v1

**Topic:** Specialist collaboration and workflow memory

## 1. What problem does it address?

Long geospatial workflows require coordinated expertise and correct dependency ordering, which can overwhelm a single copilot.

## 2. How does it solve the problem?

GeoLLM-Squad builds on GeoLLM-Engine and AutoGen, assigning specialist agents and using an orchestrator to coordinate dependencies. Intent-based tool selection and workflow memory help reuse successful execution patterns.

## 3. What experiments were conducted?

- Evaluates 2,000 prompts spanning agriculture, climate, urban analysis, forestry, and vision with GPT-4o-mini.
- Compares GeoLLM-Engine+, Chameleon, and Magentic-style systems using workflow correctness, token usage, and downstream remote sensing error measures.

## 4. What are the conclusions?

The reported correctness is 60.29 versus 43.32 for the strongest listed comparator, a gain of 16.97 percentage points. This comes with substantially higher token use in the table, and the system does not lead every downstream metric. Specialist coordination can improve reliability, but its cost matters.

**Reading pointers:** Framework and evaluation sections; Table III; PDF pages 2–5.
