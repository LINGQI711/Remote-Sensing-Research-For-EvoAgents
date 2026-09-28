# Agent Skills

[Top-level catalog](../../README.md) · [All collections](../README.md)

This collection studies **general-purpose reusable agent skills**: procedural knowledge that helps an agent act across tasks, represented as instructions, code, workflows, multimodal state-action knowledge, or retrievable modules. EO-specific skill/tool systems are indexed only in [Remote Sensing Agents](../remote-sensing-agents/README.md).

## Skill lifecycle

| Stage | Main question | Representative general-domain papers |
| --- | --- | --- |
| Representation | What is stored as a skill: text, executable code, workflow, or multimodal state? | Voyager, SkillWeaver, MMSkills, XSkill |
| Discovery | How are candidate skills proposed from exploration or trajectories? | PAE, EXIF, ASI, EvoSkill, Trace2Skill |
| Retrieval and routing | Which skill should be selected from a large library for this task? | SkillFlow, SkillCAT |
| Optimization | How should an existing skill be refined or evolved? | SkillOpt, SkillCAT, SkillWeaver |
| Learning with skills | How can skills be integrated into memory or policy learning? | MemSkill, SAGE, XSkill, Agent Workflow Memory |
| Validation | How do we reject brittle, unsafe, or task-specific skills? | EvoSkill, SkillCAT, SkillsBench |
| Evaluation | When do skills help, hurt, or transfer under realistic use? | SkillsBench, Skill Usage in the Wild, SkillFlow |

## Papers

| Paper | Skill form | Distinctive mechanism / evidence | Venue · PDF · arXiv · Code | Reading note |
| --- | --- | --- | --- | --- |
| Voyager | Executable code library | Automatic curriculum, code repair, and skill retrieval for open-ended embodied tasks | TMLR 2024 · [PDF](../../papers/general-skills/2024/TMLR/Voyager%20-%20An%20Open-Ended%20Embodied%20Agent%20with%20Large%20Language%20Models.pdf) · [arXiv](https://arxiv.org/abs/2305.16291) · [Code](https://github.com/MineDojo/Voyager) | [Note](../../notes/general-skills/Voyager.md) |
| Proposer-Agent-Evaluator (PAE) | Reusable internet-agent skills | Proposes candidate skills, executes them, and evaluates utility | arXiv preprint 2024 · [PDF](https://arxiv.org/pdf/2412.13194) · [arXiv](https://arxiv.org/abs/2412.13194) · [Project / code](https://yanqval.github.io/PAE/) | External paper |
| Agent Workflow Memory (AWM) | Reusable workflows / procedural playbooks | Induces workflows from demonstrations or online successes for later web tasks | ICML 2025 · [PDF](../../papers/general-skills/2025/ICML/Agent%20Workflow%20Memory.pdf) · [arXiv](https://arxiv.org/abs/2409.07429) · [Code](https://github.com/zorazrw/agent-workflow-memory) | [Note](../../notes/general-skills/AWM.md) |
| SkillFlow | Searchable skill library | Multi-stage retrieval and reranking over a large real-world skill corpus | COLM 2026 · [PDF](https://arxiv.org/pdf/2504.06188) · [arXiv](https://arxiv.org/abs/2504.06188) · [Code](https://github.com/IBPA/skill-flow) | External paper |
| SkillWeaver | Callable Playwright APIs | Discovers, implements, practices, and repairs reusable web skills | arXiv preprint 2025 · [PDF](../../papers/general-skills/2025/arXiv/SkillWeaver%20-%20Web%20Agents%20can%20Self-Improve%20by%20Discovering%20and%20Honing%20Skills.pdf) · [arXiv](https://arxiv.org/abs/2504.07079) · [Code](https://github.com/OSU-NLP-Group/SkillWeaver) | [Note](../../notes/general-skills/SkillWeaver.md) |
| Automated Skill Discovery through Exploration and Iterative Feedback (EXIF) | Environment-grounded skill trajectories | Exploration generates feasible skill data; evaluation feedback guides subsequent discovery | arXiv preprint 2025 · [PDF](https://arxiv.org/pdf/2506.04287) · [arXiv](https://arxiv.org/abs/2506.04287) · Code: not listed | External paper |
| Inducing Programmatic Skills for Agentic Tasks (ASI) | Programmatic skills | Induces executable skills from agentic task data | COLM 2025 · [PDF](https://arxiv.org/pdf/2504.06821) · [arXiv](https://arxiv.org/abs/2504.06821) · [Code](https://github.com/zorazrw/agent-skill-induction) | External paper |
| EvoSkill | Validated skill candidates | Executor–proposer–builder loop maintains an evidence-backed improvement frontier | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/EvoSkill%20-%20Automated%20Skill%20Discovery%20for%20Multi-Agent%20Systems.pdf) · [arXiv](https://arxiv.org/abs/2603.02766) · [Code](https://github.com/sentient-agi/EvoSkill) | [Note](../../notes/general-skills/EvoSkill.md) |
| Trace2Skill | Portable skill files | Distills trajectory-local lessons and consolidates them into transferable skills | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/Trace2Skill%20-%20Distill%20Trajectory-Local%20Lessons%20into%20Transferable%20Agent%20Skills.pdf) · [arXiv](https://arxiv.org/abs/2603.25158) · [Code](https://github.com/Qwen-Applications/Trace2Skill) | [Note](../../notes/general-skills/Trace2Skill.md) |
| XSkill | Task skills + action experiences | Continual multimodal retrieval and adaptation across task and action levels | ICML 2026 · [PDF](../../papers/general-skills/2026/ICML/XSkill%20-%20Continual%20Learning%20from%20Experience%20and%20Skills%20in%20Multimodal%20Agents.pdf) · [arXiv](https://arxiv.org/abs/2603.12056) · [Code](https://github.com/XSkill-Agent/XSkill) | [Note](../../notes/general-skills/XSkill.md) |
| Skill Usage in the Wild | Skills retrieved from a large real-world library | Tests retrieval and refinement under realistic, imperfect skill matching | arXiv preprint 2026 · [PDF](https://arxiv.org/pdf/2604.04323) · [arXiv](https://arxiv.org/abs/2604.04323) · [Code](https://github.com/UCSB-NLP-Chang/Skill-Usage) | External paper |
| SkillFlow: Benchmarking Lifelong Skill Discovery and Evolution | Sequential task families with skill discovery, patching, transfer, and library maintenance | arXiv preprint 2026 · [PDF](https://arxiv.org/pdf/2604.17308) · [arXiv](https://arxiv.org/abs/2604.17308) · [Project page](https://zhangzi-a.github.io/SkillFlow-project-page/) | External paper |
| MMSkills | Visual state cards and keyframes | Multimodal skill representation and runtime consultation | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/MMSkills%20-%20Towards%20Multimodal%20Skills%20for%20General%20Visual%20Agents.pdf) · [arXiv](https://arxiv.org/abs/2605.13527) · [Code](https://github.com/DeepExperience/MMSkills) | [Note](../../notes/general-skills/MMSkills.md) |
| SkillEvolBench | Controlled tasks for evaluating whether agents truly form and evolve reusable skills rather than replay trajectories | arXiv preprint 2026 · [PDF](https://arxiv.org/pdf/2605.24117) · [arXiv](https://arxiv.org/abs/2605.24117) · [Project page](https://skillevolbench.github.io/) | External paper |
| Skill1: Unified Evolution of Skill-Augmented Agents via Reinforcement Learning | Jointly optimizes skill retrieval, use, and distillation with a unified RL objective | arXiv preprint 2026 · [PDF](https://arxiv.org/pdf/2605.06130) · [arXiv](https://arxiv.org/abs/2605.06130) · Code: not listed | External paper |
| SkillOpt | Compact textual executive strategy | Rollout-driven skill edits with held-out acceptance | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/SkillOpt%20-%20Executive%20Strategy%20for%20Self-Evolving%20Agent%20Skills.pdf) · [arXiv](https://arxiv.org/abs/2605.23904) · [Code](https://github.com/microsoft/SkillOpt) | [Note](../../notes/general-skills/SkillOpt.md) |
| Evo-Harness: Context-to-Harness Skill Compilation for Self-Evolving Agents | Compiles transient context and successful interaction patterns into a tested, reusable skill harness while freezing the backbone | arXiv preprint 2026 · [PDF](https://arxiv.org/pdf/2608.15071) · [arXiv](https://arxiv.org/abs/2608.15071) · [Code](https://github.com/A-EVO-Lab/a-evolve/tree/release/evo-harness) | External paper |
| MemSkill | Memory operations represented as skills | Learns a controller to choose memory operations and evolve the inventory | NeurIPS 2026 · [PDF](../../papers/general-skills/2026/arXiv/MemSkill%20-%20Learning%20and%20Evolving%20Memory%20Skills%20for%20Self-Evolving%20Agents.pdf) · [arXiv](https://arxiv.org/abs/2602.02474) · [Code](https://github.com/ViktorAxelsen/MemSkill) | [Note](../../notes/general-skills/MemSkill.md) |
| SkillCAT | Hierarchical textual skills and skill topology | Contrastive extraction, patch assessment, and topology-aware routing | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/SkillCAT%20-%20Contrastive%2C%20Assessment-Augmented%20and%20Topology-Aware%20Skill%20Self-Evolution%20for%20LLM%20Agents.pdf) · [arXiv](https://arxiv.org/abs/2606.13317) · Code: not listed | [Note](../../notes/general-skills/SkillCAT.md) |
| Reinforcement Learning for Self-Improving Agent with Skill Library (SAGE) | Skill library coupled to policy learning | Sequential rollouts accumulate skills across tasks; skill-integrated reward trains skill use | arXiv preprint 2025 · [PDF](https://arxiv.org/pdf/2512.17102) · [arXiv](https://arxiv.org/abs/2512.17102) · Code: not listed | External paper |
| SkillsBench | Task–skill pairs with deterministic verifiers | Measures skill benefit and negative transfer across diverse domains | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/SkillsBench%20-%20Benchmarking%20How%20Well%20Agent%20Skills%20Work%20Across%20Diverse%20Tasks.pdf) · [arXiv](https://arxiv.org/abs/2602.12670) · [Code](https://github.com/benchflow-ai/skillsbench) | [Note](../../notes/general-skills/SkillsBench.md) |

## Research gaps

- A shared definition separating skills from prompts, demonstrations, tools, policies, workflows, and memories.
- Compositional tests where individually correct skills interfere in long workflows.
- Skill provenance, versioning, dependency tracking, safety review, and rollback.
- Cross-model and cross-environment portability without hidden adapters.
- Realistic retrieval and refinement when the exact task-specific skill is not provided.
- Cost-aware routing that trades context, latency, and task risk.

See also [Self-Evolving Agents](../self-evolving-agents/README.md), [Training-Free Agent Learning](../training-free-agent-learning/README.md), [Agent Memory](../agent-memory/README.md), and [Benchmarks and Evaluation](../benchmarks-evaluation/README.md).

