# Agent Skills

[Top-level catalog](../../README.md) · [All collections](../README.md)

This collection studies reusable procedural knowledge that changes how an agent acts. A skill may be textual guidance, an executable program, a workflow, a multimodal state-action card, a memory operation, or a structured tool-access layer.

## Skill lifecycle

| Stage | Main question | Representative papers |
| --- | --- | --- |
| Representation | What is stored as a skill? | Voyager, MMSkills, XSkill, RS-Claw |
| Discovery | How are candidate skills proposed? | SkillWeaver, EvoSkill, Trace2Skill, SkillCAT |
| Optimization | How is an existing skill revised? | SkillOpt, SkillCAT, MemSkill |
| Validation | How are harmful or task-specific skills rejected? | EvoSkill, SkillCAT, SkillOpt, SkillsBench |
| Routing | Which subset is loaded for the current state? | XSkill, SkillCAT, RS-Claw, GeoForge |
| Composition | How do atomic skills form long workflows? | Voyager, GeoForge, Earth-Agent-Pro |
| Evaluation | When does a skill help, hurt, or transfer? | SkillsBench, XSkill, GeoForge |

## Papers

| Paper | Skill form | Distinctive mechanism | Venue / PDF / arXiv / Code | Reading note |
| --- | --- | --- | --- | --- |
| Voyager | Executable code library | Automatic curriculum, code repair, and retrieval | Transactions on Machine Learning Research; [PDF](../../papers/general-skills/2024/TMLR/Voyager%20-%20An%20Open-Ended%20Embodied%20Agent%20with%20Large%20Language%20Models.pdf); [arXiv](https://arxiv.org/abs/2305.16291); [Code](https://github.com/MineDojo/Voyager) | [Note](../../notes/general-skills/Voyager.md) |
| SkillWeaver | Callable Playwright APIs | Explore, implement, practice, and hone | arXiv preprint; [PDF](../../papers/general-skills/2025/arXiv/SkillWeaver%20-%20Web%20Agents%20can%20Self-Improve%20by%20Discovering%20and%20Honing%20Skills.pdf); [arXiv](https://arxiv.org/abs/2504.07079); [Code](https://github.com/OSU-NLP-Group/SkillWeaver) | [Note](../../notes/general-skills/SkillWeaver.md) |
| EvoSkill | Validated skill candidates | Executor-proposer-builder loop and improvement frontier | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/EvoSkill%20-%20Automated%20Skill%20Discovery%20for%20Multi-Agent%20Systems.pdf); [arXiv](https://arxiv.org/abs/2603.02766); [Code](https://github.com/sentient-agi/EvoSkill) | [Note](../../notes/general-skills/EvoSkill.md) |
| MMSkills | Visual state cards and keyframes | Multimodal representation and runtime consultation | arXiv preprint 2026; [PDF](../../papers/general-skills/2026/arXiv/MMSkills%20-%20Towards%20Multimodal%20Skills%20for%20General%20Visual%20Agents.pdf); [arXiv](https://arxiv.org/abs/2605.13527); [Code](https://github.com/DeepExperience/MMSkills) | [Note](../../notes/general-skills/MMSkills.md) |
| SkillCAT | Hierarchical textual skills | Contrastive extraction, patch assessment, topology-aware routing | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/SkillCAT%20-%20Contrastive%2C%20Assessment-Augmented%20and%20Topology-Aware%20Skill%20Self-Evolution%20for%20LLM%20Agents.pdf); [arXiv](https://arxiv.org/abs/2606.13317); Code: not listed | [Note](../../notes/general-skills/SkillCAT.md) |
| SkillOpt | Compact textual executive strategy | Controlled edits, learning rate, and held-out acceptance | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/SkillOpt%20-%20Executive%20Strategy%20for%20Self-Evolving%20Agent%20Skills.pdf); [arXiv](https://arxiv.org/abs/2605.23904); [Code](https://github.com/microsoft/SkillOpt) | [Note](../../notes/general-skills/SkillOpt.md) |
| SkillsBench | Task-skill pairs with verifiers | Measures when procedural guidance helps or hurts | arXiv preprint 2026; [PDF](../../papers/general-skills/2026/arXiv/SkillsBench%20-%20Benchmarking%20How%20Well%20Agent%20Skills%20Work%20Across%20Diverse%20Tasks.pdf); [arXiv](https://arxiv.org/abs/2602.12670); [Code](https://github.com/benchflow-ai/skillsbench) | [Note](../../notes/general-skills/SkillsBench.md) |
| Trace2Skill | Portable skill directory | Parallel trajectory analysis and hierarchical consolidation | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/Trace2Skill%20-%20Distill%20Trajectory-Local%20Lessons%20into%20Transferable%20Agent%20Skills.pdf); [arXiv](https://arxiv.org/abs/2603.25158); [Code](https://github.com/Qwen-Applications/Trace2Skill) | [Note](../../notes/general-skills/Trace2Skill.md) |
| XSkill | Task skills + action experiences | Continual multimodal retrieval and adaptation | ICML 2026 (accepted); [PDF](../../papers/general-skills/2026/ICML/XSkill%20-%20Continual%20Learning%20from%20Experience%20and%20Skills%20in%20Multimodal%20Agents.pdf); [arXiv](https://arxiv.org/abs/2603.12056); [Code](https://github.com/XSkill-Agent/XSkill) | [Note](../../notes/general-skills/XSkill.md) |
| MemSkill | Memory operations as skills | Learned controller and evolving operation inventory | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/MemSkill%20-%20Learning%20and%20Evolving%20Memory%20Skills%20for%20Self-Evolving%20Agents.pdf); [arXiv](https://arxiv.org/abs/2602.02474); [Code](https://github.com/ViktorAxelsen/MemSkill) | [Note](../../notes/general-skills/MemSkill.md) |
| RS-Claw | Hierarchical tool documentation | Progressive active exploration under context limits | arXiv preprint 2026; [PDF](../../papers/remote-sensing/2026/arXiv/RS-Claw%20-%20Progressive%20Active%20Tool%20Exploration%20via%20Hierarchical%20Skill%20Trees%20for%20Remote%20Sensing%20Agents.pdf); [arXiv](https://arxiv.org/abs/2605.13391); Code: not listed | [Note](../../notes/remote-sensing/RS-Claw.md) |
| GeoForge | Adapted SOP skills | Joint use with workflow and action memories | arXiv preprint 2026; [PDF](../../papers/remote-sensing/2026/arXiv/GeoForge%20-%20Non-Parametric%20Self-Evolving%20Agents%20for%20Earth-Observation%20Reasoning.pdf); [arXiv](https://arxiv.org/abs/2608.10494); Code: not listed | [Note](../../notes/remote-sensing/GeoForge.md) |
| Earth-Agent-Pro | Expert-authored EO skills | Constrains both planning and runtime tool scope | arXiv preprint 2026; [PDF](../../papers/remote-sensing/2026/arXiv/Earth-Agent-Pro%20-%20Towards%20Real-World%20Full-Chain%20Earth%20Observation%20with%20Agents.pdf); [arXiv](https://arxiv.org/abs/2609.12533); Code: not listed | [Note](../../notes/remote-sensing/Earth-Agent-Pro.md) |

## Research gaps

- A shared definition separating skills from prompts, demonstrations, tools, policies, and memories.
- Compositional tests where individually correct skills interfere in long workflows.
- Skill provenance, versioning, dependency tracking, and rollback.
- Cross-model and cross-environment portability without hidden adapters.
- Verification when deterministic task checkers are unavailable.
- Cost-aware routing that trades context, latency, and task risk.

See also [Self-Evolving Agents](../self-evolving-agents/README.md) and [Training-Free Agent Learning](../training-free-agent-learning/README.md).
