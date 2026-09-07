# MapAgent: A Hierarchical Agent for Geospatial Reasoning with Dynamic Map Tool Integration

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/EACL-Findings/MapAgent%20-%20A%20Hierarchical%20Agent%20for%20Geospatial%20Reasoning%20with%20Dynamic%20Map%20Tool%20Integration.pdf) · [Source version](https://arxiv.org/abs/2509.05933v2) · [Publication](https://aclanthology.org/2026.findings-eacl.67/) · [Code](https://github.com/Hasebul/MapAgent)

**Venue:** Findings of EACL 2026

**Version read:** v2

**Topic:** Supporting work: hierarchical map-tool geospatial reasoning

## 1. What problem does it address?

Flat agents struggle with numerous similar map APIs and with queries requiring several dependent spatial operations. This is a map-based geospatial reasoning problem, rather than satellite-image interpretation.

## 2. How does it solve the problem?

A planner decomposes the query and routes subgoals to functional modules. A dedicated Map-Tool Agent manages tool-heavy map services, while simpler modules avoid extra agent overhead. Custom Nearby, PlaceInfo, Route, and Trip tools support coordinated sequential and parallel operations.

## 3. What experiments were conducted?

- Evaluates MapEval-Textual, MapEval-API, MapEval-Visual, and MapQA against direct-answer models and ReAct, LLMCompiler, Chameleon, and OctoTools.
- Studies multiple GPT and Qwen backbones, component ablations, errors, and execution costs.
- In the Section 5.1 ablation, accuracy is 77.44% with both custom tools and hierarchy, 56.39% without hierarchy, and 39.37% without either component.

## 4. What are the conclusions?

Hierarchical routing and task-oriented tool wrappers improve the reported map-query results. The transferable contribution is tool orchestration, not a demonstrated remote-sensing capability. Dependence on the evaluated Google Maps APIs limits claims about other services or domains.

**Reading pointers:** Sections 3-4 for architecture and benchmarks; Section 5.1 and Table 7 for ablations; Limitations. Results summarized here refer to the archived arXiv v2, not an assumed identical camera-ready version.
