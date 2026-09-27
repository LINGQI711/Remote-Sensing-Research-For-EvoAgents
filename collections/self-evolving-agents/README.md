# Self-Evolving Agents

[Top-level catalog](../../README.md) · [All collections](../README.md)

This collection focuses on **general-domain agent self-improvement**: what state changes, what interaction evidence drives the change, and how the system validates that the change transfers. Remote-sensing agents are listed exclusively in [Remote Sensing Agents](../remote-sensing-agents/README.md).

| Paper | What evolves | Evidence / safeguard | Venue · PDF · arXiv · Code | Reading note |
| --- | --- | --- | --- | --- |
| Voyager | Executable skill library and task curriculum | Environment feedback and automatic verification | TMLR 2024 · [PDF](../../papers/general-skills/2024/TMLR/Voyager%20-%20An%20Open-Ended%20Embodied%20Agent%20with%20Large%20Language%20Models.pdf) · [arXiv](https://arxiv.org/abs/2305.16291) · [Code](https://github.com/MineDojo/Voyager) | [Note](../../notes/general-skills/Voyager.md) |
| ExpeL | Natural-language insights and successful demonstrations | Learn from both successes and failures; retrieve for later tasks | AAAI 2024 · [PDF](../../papers/general-skills/2024/AAAI/ExpeL%20-%20LLM%20Agents%20Are%20Experiential%20Learners.pdf) · [arXiv](https://arxiv.org/abs/2308.10144) · [Code](https://github.com/LeapLabTHU/ExpeL) | [Note](../../notes/general-skills/ExpeL.md) |
| WebRL | Agent policy and online task curriculum | Outcome reward model, adaptive RL, and tasks generated from failures | ICLR 2025 · [PDF](https://openreview.net/attachment?id=oVKEAFjEqv&name=pdf) · [arXiv](https://arxiv.org/abs/2411.02337) · [Code](https://github.com/THUDM/WebRL) | External paper |
| SkillWeaver | Callable web-agent skills | Practice, execution, and repair on web tasks | arXiv preprint 2025 · [PDF](../../papers/general-skills/2025/arXiv/SkillWeaver%20-%20Web%20Agents%20can%20Self-Improve%20by%20Discovering%20and%20Honing%20Skills.pdf) · [arXiv](https://arxiv.org/abs/2504.07079) · [Code](https://github.com/OSU-NLP-Group/SkillWeaver) | [Note](../../notes/general-skills/SkillWeaver.md) |
| EvoSkill | Library of validated skills for multi-agent systems | Executor evidence plus candidate validation | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/EvoSkill%20-%20Automated%20Skill%20Discovery%20for%20Multi-Agent%20Systems.pdf) · [arXiv](https://arxiv.org/abs/2603.02766) · [Code](https://github.com/sentient-agi/EvoSkill) | [Note](../../notes/general-skills/EvoSkill.md) |
| SkillOpt | Compact textual executive strategy | Rollout-based edits with held-out acceptance | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/SkillOpt%20-%20Executive%20Strategy%20for%20Self-Evolving%20Agent%20Skills.pdf) · [arXiv](https://arxiv.org/abs/2605.23904) · [Code](https://github.com/microsoft/SkillOpt) | [Note](../../notes/general-skills/SkillOpt.md) |
| SkillCAT | Hierarchical skill topology and skill contents | Contrastive outcomes, assessment, and topology-aware routing | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/SkillCAT%20-%20Contrastive%2C%20Assessment-Augmented%20and%20Topology-Aware%20Skill%20Self-Evolution%20for%20LLM%20Agents.pdf) · [arXiv](https://arxiv.org/abs/2606.13317) · Code: not listed | [Note](../../notes/general-skills/SkillCAT.md) |

## Mechanism questions

- **State:** Does the agent modify memory, a skill library, workflows, tools, curriculum, or parameters?
- **Signal:** Are updates based on outcome reward, process verification, critique, or human feedback?
- **Validation:** Are candidate changes replay-tested and accepted only on held-out tasks?
- **Safety:** How are regressions, reward hacking, stale skills, and negative transfer detected?
- **Attribution:** Can the gain be tied to the changed component rather than extra inference compute?

See also [Training-Free Agent Learning](../training-free-agent-learning/README.md), [Agent Skills](../agent-skills/README.md), and [Agent Training and RL](../agent-training-rl/README.md).
