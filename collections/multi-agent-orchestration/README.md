# Multi-Agent and Orchestration

[Top-level catalog](../../README.md) · [All collections](../README.md)

This collection presents **general-domain** multi-agent systems and coordination methods. EO/geospatial multi-agent systems appear only in [Remote Sensing Agents](../remote-sensing-agents/README.md).

## Research storyline

Multi-agent systems vary along three axes: **who is assigned a role**, **how work and state move between agents**, and **whether the topology is fixed or chosen dynamically**. Early systems establish role-play and conversational coordination; SOPs and artifacts make handoffs more structured; newer orchestrators emphasize a manager, specialist routing, or a mixed human/agent team. More agents do not automatically mean better results: compare with a single agent under equal total model, token, tool-call, and wall-clock budgets.

| Paper | Organization / mechanism | Venue · PDF · arXiv · Code | Reading note |
| --- | --- | --- | --- |
| CAMEL | Role-playing agents coordinate through communicative interaction | NeurIPS 2023 · [PDF](https://arxiv.org/pdf/2303.17760) · [arXiv](https://arxiv.org/abs/2303.17760) · [Code](https://github.com/camel-ai/camel) | External paper |
| MetaGPT | SOP-driven software-company roles with structured artifacts and handoffs | ICLR 2024 · [PDF](https://arxiv.org/pdf/2308.00352) · [arXiv](https://arxiv.org/abs/2308.00352) · [Code](https://github.com/geekan/MetaGPT) | External paper |
| AutoGen | Conversable agents and programmable group-chat orchestration | arXiv preprint / technical report 2023 · [PDF](https://arxiv.org/pdf/2308.08155) · [arXiv](https://arxiv.org/abs/2308.08155) · [Code](https://github.com/microsoft/autogen) | External paper |
| AgentVerse | Configurable multi-agent collaboration and emergent role specialization | arXiv preprint 2023 · [PDF](https://arxiv.org/pdf/2308.10848) · [arXiv](https://arxiv.org/abs/2308.10848) · [Code](https://github.com/OpenBMB/AgentVerse) | External paper |
| ChatDev | Virtual software company in which role-based agents collaborate through a structured software-development process | ACL 2024 · [PDF](https://aclanthology.org/2024.acl-long.810.pdf) · [arXiv](https://arxiv.org/abs/2307.07924) · [Code](https://github.com/OpenBMB/ChatDev) | External paper |
| Magentic-One | Generalist manager coordinates a planner, web/computer specialists, and a file agent using task ledger and progress ledger | arXiv technical report 2024 · [PDF](https://www.microsoft.com/en-us/research/wp-content/uploads/2024/11/MagenticOne.pdf) · [arXiv](https://arxiv.org/abs/2411.04468) · [Code](https://github.com/microsoft/autogen) | External paper |
| Multi-agent Architecture Search via Agentic Supernet (MaAS) | Samples query-specific collaboration architectures from a probabilistic supernet, allocating agents and inference cost to task difficulty | ICML 2025 · [PDF](https://proceedings.mlr.press/v267/zhang25bi/zhang25bi.pdf) · [arXiv](https://arxiv.org/abs/2502.04180) · [Code](https://github.com/bingreeky/MaAS) | External paper |
| AgentNet: Decentralized Evolutionary Coordination for LLM-based Multi-Agent Systems | Replaces a fixed central controller with a dynamically evolving agent DAG, local routing, and retrieval-based specialization | NeurIPS 2025 · [PDF](https://papers.nips.cc/paper_files/paper/2025/file/9a379c1b05793d1c42dc832269834515-Paper-Conference.pdf) · [arXiv](https://arxiv.org/abs/2504.00587) · [Code](https://github.com/zoe-yyx/agentnet) | External paper |
| Multi-Agent Collaboration via Evolving Orchestration | Learns a centralized “puppeteer” policy with RL to activate and sequence agents as task state changes | NeurIPS 2025 · [PDF](https://proceedings.neurips.cc/paper_files/paper/2025/file/f1320d2e2842169c6fc89dcbd80e94d0-Paper-Conference.pdf) · [arXiv](https://arxiv.org/abs/2505.19591) · [Code](https://github.com/OpenBMB/ChatDev/tree/puppeteer) | External paper |
| EvoSkill | Executor, proposer, and skill-builder loop for multi-agent skill discovery | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/EvoSkill%20-%20Automated%20Skill%20Discovery%20for%20Multi-Agent%20Systems.pdf) · [arXiv](https://arxiv.org/abs/2603.02766) · [Code](https://github.com/sentient-agi/EvoSkill) | [Note](../../notes/general-skills/EvoSkill.md) |
| RAAS: LLM Agentic System Architecture Search with GRPO | Stabilizes architecture search using same-query peer comparison and multi-trial assessment, reducing task-difficulty and execution-noise bias | CVPR 2026 · [PDF](https://openaccess.thecvf.com/content/CVPR2026/papers/Yang_RAAS_LLM_Agentic_System_Architecture_Search_with_GRPO_CVPR_2026_paper.pdf) · arXiv: not listed · [Code](https://github.com/ridlog/raas) | External paper |

## Reading path

Read **CAMEL / AgentVerse** for role-play and group collaboration, **MetaGPT / ChatDev** for process- and artifact-mediated handoffs, and **AutoGen / Magentic-One** for programmable conversation and manager-led specialist orchestration. For current research, compare **MaAS → AgentNet → Evolving Orchestration → RAAS**: query-conditioned architecture sampling, decentralized topology evolution, RL-trained centralized routing, and more robust architecture-search evaluation. **EvoSkill** links coordination to reusable skill evolution. Across all of them, distinguish coordination gains from duplicated reasoning, communication overhead, and a stronger backbone; compare under matched total inference budgets.

## Coordination patterns and controls

| Pattern | Benefit sought | Common risk |
| --- | --- | --- |
| Manager-worker | Long-horizon decomposition and routing | Bottlenecks and cascading plan errors |
| Specialist roles | Expertise and reduced action space | Inconsistent assumptions and costly handoffs |
| Debate / critique | Error detection and uncertainty exposure | Persuasive but ungrounded consensus |
| Planner-executor | Separate global planning from local action | Plan-execution mismatch |
| Proposer-validator | Controlled self-improvement | Validator bias and overfitting to known checks |

Compare against a single agent under the same total token/tool budget; measure communication value, error propagation, recovery, and delegation decisions.

