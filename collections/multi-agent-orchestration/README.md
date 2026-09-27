# Multi-Agent and Orchestration

[Top-level catalog](../../README.md) · [All collections](../README.md)

This collection presents **general-domain** multi-agent systems and coordination methods. EO/geospatial multi-agent systems appear only in [Remote Sensing Agents](../remote-sensing-agents/README.md).

| Paper | Organization / mechanism | Venue · PDF · arXiv · Code | Reading note |
| --- | --- | --- | --- |
| CAMEL | Role-playing agents coordinate through communicative interaction | NeurIPS 2023 · [PDF](https://arxiv.org/pdf/2303.17760) · [arXiv](https://arxiv.org/abs/2303.17760) · [Code](https://github.com/camel-ai/camel) | External paper |
| MetaGPT | SOP-driven software-company roles with structured artifacts and handoffs | ICLR 2024 · [PDF](https://arxiv.org/pdf/2308.00352) · [arXiv](https://arxiv.org/abs/2308.00352) · [Code](https://github.com/geekan/MetaGPT) | External paper |
| AutoGen | Conversable agents and programmable group-chat orchestration | arXiv preprint / technical report 2023 · [PDF](https://arxiv.org/pdf/2308.08155) · [arXiv](https://arxiv.org/abs/2308.08155) · [Code](https://github.com/microsoft/autogen) | External paper |
| AgentVerse | Configurable multi-agent collaboration and emergent role specialization | arXiv preprint 2023 · [PDF](https://arxiv.org/pdf/2308.10848) · [arXiv](https://arxiv.org/abs/2308.10848) · [Code](https://github.com/OpenBMB/AgentVerse) | External paper |
| EvoSkill | Executor, proposer, and skill-builder loop for multi-agent skill discovery | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/EvoSkill%20-%20Automated%20Skill%20Discovery%20for%20Multi-Agent%20Systems.pdf) · [arXiv](https://arxiv.org/abs/2603.02766) · [Code](https://github.com/sentient-agi/EvoSkill) | [Note](../../notes/general-skills/EvoSkill.md) |

## Coordination patterns and controls

| Pattern | Benefit sought | Common risk |
| --- | --- | --- |
| Manager-worker | Long-horizon decomposition and routing | Bottlenecks and cascading plan errors |
| Specialist roles | Expertise and reduced action space | Inconsistent assumptions and costly handoffs |
| Debate / critique | Error detection and uncertainty exposure | Persuasive but ungrounded consensus |
| Planner-executor | Separate global planning from local action | Plan-execution mismatch |
| Proposer-validator | Controlled self-improvement | Validator bias and overfitting to known checks |

Compare against a single agent under the same total token/tool budget; measure communication value, error propagation, recovery, and delegation decisions.
