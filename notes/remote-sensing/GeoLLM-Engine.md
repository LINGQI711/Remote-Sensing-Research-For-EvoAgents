# GeoLLM-Engine: A Realistic Environment for Building Geospatial Copilots

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2024/CVPR-Workshops/GeoLLM-Engine%20-%20A%20Realistic%20Environment%20for%20Building%20Geospatial%20Copilots.pdf) · [Source version](https://arxiv.org/abs/2404.15500v1)

**Venue:** CVPR 2024 Workshops · EarthVision

**Version read:** v1

**Topic:** Executable environments for geospatial copilots

## 1. What problem does it address?

Simple demonstrations do not capture the breadth, dependencies, and state changes of real geospatial workflows.

## 2. How does it solve the problem?

GeoLLM-Engine supplies more than 175 tools spanning imagery, databases, mapping interfaces, and external knowledge. A formal environment state and model checking support executable workflows and automatically constructed evaluation queries.

## 3. What experiments were conducted?

- Compares GPT-3.5 and GPT-4 Turbo with Chameleon, chain-of-thought, and ReAct-style prompting, measuring correctness, functional success, and token consumption.
- Scales from 10,000 queries containing 50,830 tool tasks to 100,000 queries containing 521,868 tool tasks. These are tool-level tasks, not half a million independent user queries.
- Analyzes longer workflows and their tool-count dependencies.

## 4. What are the conclusions?

Environment coverage and workflow complexity expose failures hidden by small demonstrations. Scaling query volume has a modest effect in one GPT-4 configuration, while workflows with many tools remain difficult. The contribution is realistic infrastructure for copilot evaluation, rather than an experience-learning algorithm.

**Reading pointers:** Sections 3–4; Tables 4–5; PDF pages 3–8.
