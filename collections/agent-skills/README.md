# Agent Skills

[Top-level catalog](../../README.md) · [All collections](../README.md)

This collection is about **general-purpose reusable agent skills**: their representation, discovery, refinement, validation, routing, and composition. Remote-sensing tool manuals and EO-specific skills are indexed only in [Remote Sensing Agents](../remote-sensing-agents/README.md).

| Paper | Skill representation / contribution | Venue · PDF · arXiv · Code | Reading note |
| --- | --- | --- | --- |
| Voyager | Executable code skills with an automatic curriculum and iterative repair | TMLR 2024 · [PDF](../../papers/general-skills/2024/TMLR/Voyager%20-%20An%20Open-Ended%20Embodied%20Agent%20with%20Large%20Language%20Models.pdf) · [arXiv](https://arxiv.org/abs/2305.16291) · [Code](https://github.com/MineDojo/Voyager) | [Note](../../notes/general-skills/Voyager.md) |
| Proposer-Agent-Evaluator (PAE) | Proposes, executes, and evaluates reusable skills for internet agents | arXiv preprint 2024 · [PDF](https://arxiv.org/pdf/2412.13194) · [arXiv](https://arxiv.org/abs/2412.13194) · [Project / code](https://yanqval.github.io/PAE/) | External paper |
| SkillWeaver | Callable Playwright APIs discovered and honed through practice | arXiv preprint 2025 · [PDF](../../papers/general-skills/2025/arXiv/SkillWeaver%20-%20Web%20Agents%20can%20Self-Improve%20by%20Discovering%20and%20Honing%20Skills.pdf) · [arXiv](https://arxiv.org/abs/2504.07079) · [Code](https://github.com/OSU-NLP-Group/SkillWeaver) | [Note](../../notes/general-skills/SkillWeaver.md) |
| Inducing Programmatic Skills for Agentic Tasks (ASI) | Programmatic skills induced from agentic task data | COLM 2025 · [PDF](https://arxiv.org/pdf/2504.06821) · [arXiv](https://arxiv.org/abs/2504.06821) · [Code](https://github.com/zorazrw/agent-skill-induction) | External paper |
| EvoSkill | Validated skill frontier for multi-agent systems | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/EvoSkill%20-%20Automated%20Skill%20Discovery%20for%20Multi-Agent%20Systems.pdf) · [arXiv](https://arxiv.org/abs/2603.02766) · [Code](https://github.com/sentient-agi/EvoSkill) | [Note](../../notes/general-skills/EvoSkill.md) |
| Trace2Skill | Portable skill files distilled and consolidated from trajectories | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/Trace2Skill%20-%20Distill%20Trajectory-Local%20Lessons%20into%20Transferable%20Agent%20Skills.pdf) · [arXiv](https://arxiv.org/abs/2603.25158) · [Code](https://github.com/Qwen-Applications/Trace2Skill) | [Note](../../notes/general-skills/Trace2Skill.md) |
| SkillOpt | Text-based executive strategy with rollout-driven optimization | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/SkillOpt%20-%20Executive%20Strategy%20for%20Self-Evolving%20Agent%20Skills.pdf) · [arXiv](https://arxiv.org/abs/2605.23904) · [Code](https://github.com/microsoft/SkillOpt) | [Note](../../notes/general-skills/SkillOpt.md) |
| MMSkills | Visual state cards and keyframes for multimodal agents | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/MMSkills%20-%20Towards%20Multimodal%20Skills%20for%20General%20Visual%20Agents.pdf) · [arXiv](https://arxiv.org/abs/2605.13527) · [Code](https://github.com/DeepExperience/MMSkills) | [Note](../../notes/general-skills/MMSkills.md) |
| SkillsBench | Evaluates when reusable skills help or hurt across diverse tasks | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/SkillsBench%20-%20Benchmarking%20How%20Well%20Agent%20Skills%20Work%20Across%20Diverse%20Tasks.pdf) · [arXiv](https://arxiv.org/abs/2602.12670) · [Code](https://github.com/benchflow-ai/skillsbench) | [Note](../../notes/general-skills/SkillsBench.md) |

## Skill lifecycle

| Stage | Core question |
| --- | --- |
| Representation | Is a skill prose, a procedure, executable code, a visual state, or a composable tool? |
| Discovery | How are candidates proposed from demonstrations, exploration, or task traces? |
| Validation | What evidence rejects brittle, unsafe, or task-specific skills? |
| Routing | Which skill should be loaded for the current state and context budget? |
| Composition | How do atomic skills form reliable long-horizon workflows? |
| Evaluation | Do skills improve held-out transfer, and what regressions do they cause? |

See also [Self-Evolving Agents](../self-evolving-agents/README.md) and [Benchmarks and Evaluation](../benchmarks-evaluation/README.md).
