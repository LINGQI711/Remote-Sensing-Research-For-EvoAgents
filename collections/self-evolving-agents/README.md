# Self-Evolving Agents

[Top-level catalog](../../README.md) · [All collections](../README.md)

This collection uses *self-evolution* narrowly: interaction evidence must change a reusable component that affects later tasks. The changed component may be memory, a skill, a workflow, a tool, or a learned controller. Repeated retries without persistent state are not evolution.

## Evolution mechanisms

| Paper | Evolving object | Candidate generation | Acceptance/control | Venue / PDF / arXiv / Code | Reading note |
| --- | --- | --- | --- | --- | --- |
| SkillWeaver | Callable web skills | Exploration and implementation | Practice and repair through execution | arXiv preprint; [PDF](../../papers/general-skills/2025/arXiv/SkillWeaver%20-%20Web%20Agents%20can%20Self-Improve%20by%20Discovering%20and%20Honing%20Skills.pdf); [arXiv](https://arxiv.org/abs/2504.07079); [Code](https://github.com/OSU-NLP-Group/SkillWeaver) | [Note](../../notes/general-skills/SkillWeaver.md) |
| EvoSkill | Multi-agent skill set | Proposer and skill builder | Validation frontier | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/EvoSkill%20-%20Automated%20Skill%20Discovery%20for%20Multi-Agent%20Systems.pdf); [arXiv](https://arxiv.org/abs/2603.02766); [Code](https://github.com/sentient-agi/EvoSkill) | [Note](../../notes/general-skills/EvoSkill.md) |
| SkillCAT | Hierarchical skill patches | Contrastive causal extraction | Replay assessment before merging | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/SkillCAT%20-%20Contrastive%2C%20Assessment-Augmented%20and%20Topology-Aware%20Skill%20Self-Evolution%20for%20LLM%20Agents.pdf); [arXiv](https://arxiv.org/abs/2606.13317); Code: not listed | [Note](../../notes/general-skills/SkillCAT.md) |
| SkillOpt | Textual executive skill | Bounded rollout-and-reflection edits | Held-out acceptance + rejected-edit memory | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/SkillOpt%20-%20Executive%20Strategy%20for%20Self-Evolving%20Agent%20Skills.pdf); [arXiv](https://arxiv.org/abs/2605.23904); [Code](https://github.com/microsoft/SkillOpt) | [Note](../../notes/general-skills/SkillOpt.md) |
| MemSkill | Memory skill inventory | Designer proposes new/refined operations | Controller optimization and task evidence | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/MemSkill%20-%20Learning%20and%20Evolving%20Memory%20Skills%20for%20Self-Evolving%20Agents.pdf); [arXiv](https://arxiv.org/abs/2602.02474); [Code](https://github.com/ViktorAxelsen/MemSkill) | [Note](../../notes/general-skills/MemSkill.md) |
| Trace2Skill | Portable skill directory | Parallel trace analysts | Hierarchical consolidation | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/Trace2Skill%20-%20Distill%20Trajectory-Local%20Lessons%20into%20Transferable%20Agent%20Skills.pdf); [arXiv](https://arxiv.org/abs/2603.25158); [Code](https://github.com/Qwen-Applications/Trace2Skill) | [Note](../../notes/general-skills/Trace2Skill.md) |
| XSkill | Skills and experiences | Trajectory distillation | Retrieval-time reuse and adaptation | ICML 2026 (accepted); [PDF](../../papers/general-skills/2026/ICML/XSkill%20-%20Continual%20Learning%20from%20Experience%20and%20Skills%20in%20Multimodal%20Agents.pdf); [arXiv](https://arxiv.org/abs/2603.12056); [Code](https://github.com/XSkill-Agent/XSkill) | [Note](../../notes/general-skills/XSkill.md) |
| GeoEvolver | Contextual EO constraints | Multi-agent parameter exploration | Success/failure contrast and root-cause analysis | arXiv preprint; [PDF](../../papers/remote-sensing/2026/arXiv/Experience-Driven%20Multi-Agent%20Systems%20Are%20Training-free%20Context-aware%20Earth%20Observers.pdf); [arXiv](https://arxiv.org/abs/2602.02559); Code: not listed | [Note](../../notes/remote-sensing/GeoEvolver.md) |
| GeoForge | Graph, experience, and SOP memories | Post-task distillation | Safety gate and reliability pruning | arXiv preprint 2026; [PDF](../../papers/remote-sensing/2026/arXiv/GeoForge%20-%20Non-Parametric%20Self-Evolving%20Agents%20for%20Earth-Observation%20Reasoning.pdf); [arXiv](https://arxiv.org/abs/2608.10494); Code: not listed | [Note](../../notes/remote-sensing/GeoForge.md) |
| RSMeM | Knowledge-grounded execution memory | Failure-aware reflection | Compression and repeated-task refinement | ACL 2026; [PDF](../../papers/remote-sensing/2026/ACL/RSMeM%20-%20Knowledge-Enhanced%20Memory%20Evolution%20for%20Remote%20Sensing%20Agents%20with%20Systematic%20Evaluation.pdf); [arXiv](https://arxiv.org/abs/2607.24772); [Code](https://github.com/AI9Stars/RSMeM) | [Note](../../notes/remote-sensing/RSMeM.md) |
| GeoEvolve | Geospatial algorithms | Multi-agent model discovery | Validation of discovered candidates | arXiv preprint 2025; [PDF](../../papers/remote-sensing/2025/arXiv/GeoEvolve%20-%20Automating%20Geospatial%20Model%20Discovery%20via%20Multi-Agent%20Large%20Language%20Models.pdf); [arXiv](https://arxiv.org/abs/2509.21593); Code: not listed | [Note](../../notes/remote-sensing/GeoEvolve.md) |

## Evaluation checklist

1. State what changes and whether model weights remain frozen.
2. Separate same-task retries from transfer to unseen tasks.
3. Report the source, amount, and order of evolution experience.
4. Test harmful updates, rollback, and conflict resolution.
5. Compare against more retries, longer context, retrieval-only, and parameter-update baselines.
6. Measure retained performance after multiple updates, not only the final task.

## Research gaps

- Evolution credit assignment across task, workflow, and action levels.
- Safe acceptance gates that do not depend on unavailable ground truth.
- Open-ended growth without unbounded memory and context cost.
- Cross-domain evolution that preserves scientific or physical constraints.
- Reproducible continual protocols with temporal ordering and contamination controls.

See also [Agent Skills](../agent-skills/README.md), [Agent Memory](../agent-memory/README.md), and [Benchmarks and Evaluation](../benchmarks-evaluation/README.md).
