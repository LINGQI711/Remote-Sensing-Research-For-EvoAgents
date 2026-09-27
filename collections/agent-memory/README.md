# Agent Memory

[Top-level catalog](../../README.md) · [All collections](../README.md)

Agent memory is treated here as a stateful mechanism with explicit write, retrieve, update, compression, or forgetting operations. Merely placing the current trajectory in a context window is not sufficient.

## Memory systems in the library

| Paper | Memory unit | Write/update mechanism | Retrieval/use | Venue / PDF / arXiv / Code | Reading note |
| --- | --- | --- | --- | --- | --- |
| ExpeL | Insights and successful demonstrations | Extracted from successes and failures | Similarity-based experience retrieval | AAAI 2024; [PDF](../../papers/general-skills/2024/AAAI/ExpeL%20-%20LLM%20Agents%20Are%20Experiential%20Learners.pdf); [arXiv](https://arxiv.org/abs/2308.10144); [Code](https://github.com/LeapLabTHU/ExpeL) | [Note](../../notes/general-skills/ExpeL.md) |
| AWM | Reusable workflows | Induced offline or from online successes | Added to later task context | ICML 2025; [PDF](../../papers/general-skills/2025/ICML/Agent%20Workflow%20Memory.pdf); [arXiv](https://arxiv.org/abs/2409.07429); [Code](https://github.com/zorazrw/agent-workflow-memory) | [Note](../../notes/general-skills/AWM.md) |
| MemSkill | Memory operations as skills | Designer adds/refines skills; controller is optimized | Controller selects memory skills | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/MemSkill%20-%20Learning%20and%20Evolving%20Memory%20Skills%20for%20Self-Evolving%20Agents.pdf); [arXiv](https://arxiv.org/abs/2602.02474); [Code](https://github.com/ViktorAxelsen/MemSkill) | [Note](../../notes/general-skills/MemSkill.md) |
| XSkill | Task-level skills and action-level experiences | Distilled from visual trajectories | Retrieve and adapt both levels | ICML 2026 (accepted); [PDF](../../papers/general-skills/2026/ICML/XSkill%20-%20Continual%20Learning%20from%20Experience%20and%20Skills%20in%20Multimodal%20Agents.pdf); [arXiv](https://arxiv.org/abs/2603.12056); [Code](https://github.com/XSkill-Agent/XSkill) | [Note](../../notes/general-skills/XSkill.md) |
| GeoEvolver | Contextual tool constraints | Root-cause attribution over explored trajectories | Retrieved for later sub-goals | arXiv preprint; [PDF](../../papers/remote-sensing/2026/arXiv/Experience-Driven%20Multi-Agent%20Systems%20Are%20Training-free%20Context-aware%20Earth%20Observers.pdf); [arXiv](https://arxiv.org/abs/2602.02559); Code: not listed | [Note](../../notes/remote-sensing/GeoEvolver.md) |
| GeoForge | Workflow graph, action experiences, skill SOPs | Safety-gated post-task distillation | Task-conditioned multi-memory prior | arXiv preprint 2026; [PDF](../../papers/remote-sensing/2026/arXiv/GeoForge%20-%20Non-Parametric%20Self-Evolving%20Agents%20for%20Earth-Observation%20Reasoning.pdf); [arXiv](https://arxiv.org/abs/2608.10494); Code: not listed | [Note](../../notes/remote-sensing/GeoForge.md) |
| RSMeM | Hierarchical domain knowledge + compact failure experience | Failure-aware refinement and trace compression | Knowledge grounding plus reusable constraints | ACL 2026; [PDF](../../papers/remote-sensing/2026/ACL/RSMeM%20-%20Knowledge-Enhanced%20Memory%20Evolution%20for%20Remote%20Sensing%20Agents%20with%20Systematic%20Evaluation.pdf); [arXiv](https://arxiv.org/abs/2607.24772); [Code](https://github.com/AI9Stars/RSMeM) | [Note](../../notes/remote-sensing/RSMeM.md) |
| Earth-Agent-Pro | Planned workflow, accepted evidence, and dependencies | Updated after verified execution | Preserves valid prefixes and repairs invalid suffixes | arXiv preprint 2026; [PDF](../../papers/remote-sensing/2026/arXiv/Earth-Agent-Pro%20-%20Towards%20Real-World%20Full-Chain%20Earth%20Observation%20with%20Agents.pdf); [arXiv](https://arxiv.org/abs/2609.12533); Code: not listed | [Note](../../notes/remote-sensing/Earth-Agent-Pro.md) |
| Multi-Agent Geospatial Copilots | Workflow memory | Stores reusable specialist workflows | Supports later orchestration | IGARSS 2025; [PDF](../../papers/remote-sensing/2025/IGARSS/Multi-Agent%20Geospatial%20Copilots%20for%20Remote%20Sensing%20Workflows.pdf); [arXiv](https://arxiv.org/abs/2501.16254); Code: not listed | [Note](../../notes/remote-sensing/Multi-Agent-Geospatial-Copilots.md) |

## Design axes

| Axis | Alternatives to compare |
| --- | --- |
| Representation | Text lesson, demonstration, key-value record, workflow graph, executable program, multimodal trace |
| Granularity | Token/action, tool call, sub-goal, task, workflow, domain |
| Write policy | Every trajectory, only successes, failures only, contrastive pairs, verifier-gated updates |
| Retrieval | Semantic similarity, topology, task type, tool constraints, uncertainty, learned controller |
| Maintenance | Append-only, merge, compress, revise, decay, forget, conflict resolution |
| Evaluation | Immediate gain, held-out transfer, retention, negative transfer, token cost, contamination resistance |

## Research gaps

- Causal attribution: identify which stored item changed a later decision.
- Memory consolidation across heterogeneous tools and modalities without erasing rare constraints.
- Adversarial and low-quality experience filtering.
- Calibrated forgetting when tools, APIs, or environments change.
- Matched comparisons between external memory and parameter-efficient fine-tuning.

See also [Training-Free Agent Learning](../training-free-agent-learning/README.md) and [Self-Evolving Agents](../self-evolving-agents/README.md).
