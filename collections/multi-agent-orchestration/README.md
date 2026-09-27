# Multi-Agent and Orchestration

[Top-level catalog](../../README.md) · [All collections](../README.md)

This collection studies systems that separate responsibilities across agents or roles. The key research issue is not the number of prompts, but whether coordination improves decomposition, verification, expertise, and recovery enough to justify communication and execution cost.

## Systems

| Paper | Organization | Coordination mechanism | Venue / PDF / arXiv / Code | Reading note |
| --- | --- | --- | --- | --- |
| Multi-Agent Geospatial Copilots | Specialist copilots | Workflow memory and domain-specialist collaboration | IGARSS 2025; [PDF](../../papers/remote-sensing/2025/IGARSS/Multi-Agent%20Geospatial%20Copilots%20for%20Remote%20Sensing%20Workflows.pdf); [arXiv](https://arxiv.org/abs/2501.16254); Code: not listed | [Note](../../notes/remote-sensing/Multi-Agent-Geospatial-Copilots.md) |
| GeoEvolve | Discovery and validation agents | Multi-agent geospatial algorithm search | arXiv preprint 2025; [PDF](../../papers/remote-sensing/2025/arXiv/GeoEvolve%20-%20Automating%20Geospatial%20Model%20Discovery%20via%20Multi-Agent%20Large%20Language%20Models.pdf); [arXiv](https://arxiv.org/abs/2509.21593); Code: not listed | [Note](../../notes/remote-sensing/GeoEvolve.md) |
| GeoEvolver | Orchestrator + exploring agents | Sub-goal decomposition and parameter exploration | arXiv preprint; [PDF](../../papers/remote-sensing/2026/arXiv/Experience-Driven%20Multi-Agent%20Systems%20Are%20Training-free%20Context-aware%20Earth%20Observers.pdf); [arXiv](https://arxiv.org/abs/2602.02559); Code: not listed | [Note](../../notes/remote-sensing/GeoEvolver.md) |
| HiRS-Agent | Manager + specialists | Routing, verification, replanning, and hierarchical objectives | ACM Multimedia 2026 (accepted); [PDF](../../papers/remote-sensing/2026/ACM-MM/HiRS-Agent%20-%20A%20Hierarchical%20Multi-Agent%20System%20for%20Reliable%20Long-Horizon%20Remote%20Sensing%20Task%20Solving.pdf); [arXiv](https://arxiv.org/abs/2608.30672); Code: not listed | [Note](../../notes/remote-sensing/HiRS-Agent.md) |
| GeoMMAgent | Coordinated geoscience specialists | Tool-supported expert reasoning | CVPR 2026 (Highlight); [PDF](../../papers/remote-sensing/2026/CVPR/GeoMMBench%20and%20GeoMMAgent%20-%20Toward%20Expert-Level%20Multimodal%20Intelligence%20in%20Geoscience%20and%20Remote%20Sensing.pdf); [arXiv](https://arxiv.org/abs/2604.08896); [Code](https://github.com/Shihao-Cheng/GeoMMAgent) | [Note](../../notes/remote-sensing/GeoMMAgent.md) |
| GaiaAgent | Task-specific agents | Coordinated 2D/3D change analysis | ISPRS Journal of Photogrammetry and Remote Sensing; [PDF](../../papers/remote-sensing/2026/ISPRS-JPRS/Towards%20comprehensive%20multi-task%20land%20cover%20change%20detection%20leveraging%20vision-language%20model%20and%20LLM-driven%20agents.pdf); arXiv: none; Code: not listed | [Note](../../notes/remote-sensing/GaiaAgent.md) |
| MapAgent | Hierarchical agent roles | Dynamic map-tool integration | Findings of EACL 2026; [PDF](../../papers/remote-sensing/2026/EACL-Findings/MapAgent%20-%20A%20Hierarchical%20Agent%20for%20Geospatial%20Reasoning%20with%20Dynamic%20Map%20Tool%20Integration.pdf); [arXiv](https://arxiv.org/abs/2509.05933); [Code](https://github.com/Hasebul/MapAgent) | [Note](../../notes/remote-sensing/MapAgent.md) |
| Earth-Agent-Pro | Planner + Executor roles | Shared skills, evidence memory, and workflow repair | arXiv preprint 2026; [PDF](../../papers/remote-sensing/2026/arXiv/Earth-Agent-Pro%20-%20Towards%20Real-World%20Full-Chain%20Earth%20Observation%20with%20Agents.pdf); [arXiv](https://arxiv.org/abs/2609.12533); Code: not listed | [Note](../../notes/remote-sensing/Earth-Agent-Pro.md) |
| EvoSkill | Executor + proposer + skill builder | Candidate generation and validation frontier | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/EvoSkill%20-%20Automated%20Skill%20Discovery%20for%20Multi-Agent%20Systems.pdf); [arXiv](https://arxiv.org/abs/2603.02766); [Code](https://github.com/sentient-agi/EvoSkill) | [Note](../../notes/general-skills/EvoSkill.md) |

## Coordination patterns

| Pattern | Benefit sought | Common risk |
| --- | --- | --- |
| Manager-worker | Long-horizon decomposition and routing | Manager bottleneck and cascading plan errors |
| Domain specialists | Expertise and reduced action space | Inconsistent assumptions and costly handoffs |
| Parallel exploration | Diverse tools, parameters, or solutions | Duplicate work and difficult credit assignment |
| Debate/critique | Error detection and uncertainty exposure | Persuasive consensus without grounded evidence |
| Planner-executor | Separate global workflow from local grounding | Plan-execution mismatch |
| Proposer-validator | Controlled self-improvement | Validator bias and overfitting to known checks |

## Research gaps

- Compare against a single agent with the same total token and tool budget.
- Measure communication value per message, not only final performance.
- Trace error propagation across role boundaries.
- Learn when to delegate, merge, stop, or escalate to a human.
- Maintain shared evidence and state without contradictory private memories.

See also [Agent Memory](../agent-memory/README.md) and [Benchmarks and Evaluation](../benchmarks-evaluation/README.md).
