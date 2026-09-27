# Training-Free Agent Learning

[Top-level catalog](../../README.md) · [All collections](../README.md)

This collection studies improvement **without updating the backbone model during the target task sequence**. Learning state lives in prompts, memories, demonstrations, workflows, skills, programs, tools, or retrieval indexes. Some papers may use an already-trained model or offline preparation; the classification concerns the adaptation mechanism being studied.

## Core papers

| Paper | Adaptation state | Update signal | Main evidence | Venue / PDF / arXiv / Code | Reading note |
| --- | --- | --- | --- | --- | --- |
| ExpeL | Natural-language insights + successful demonstrations | Success/failure trajectories | Cross-task experiential reuse | AAAI 2024; [PDF](../../papers/general-skills/2024/AAAI/ExpeL%20-%20LLM%20Agents%20Are%20Experiential%20Learners.pdf); [arXiv](https://arxiv.org/abs/2308.10144); [Code](https://github.com/LeapLabTHU/ExpeL) | [Note](../../notes/general-skills/ExpeL.md) |
| Voyager | Executable skill library | Environment feedback + self-verification | Open-ended curriculum and skill reuse | Transactions on Machine Learning Research; [PDF](../../papers/general-skills/2024/TMLR/Voyager%20-%20An%20Open-Ended%20Embodied%20Agent%20with%20Large%20Language%20Models.pdf); [arXiv](https://arxiv.org/abs/2305.16291); [Code](https://github.com/MineDojo/Voyager) | [Note](../../notes/general-skills/Voyager.md) |
| AWM | Reusable workflow memory | Offline examples or online successful episodes | Web-task transfer | ICML 2025; [PDF](../../papers/general-skills/2025/ICML/Agent%20Workflow%20Memory.pdf); [arXiv](https://arxiv.org/abs/2409.07429); [Code](https://github.com/zorazrw/agent-workflow-memory) | [Note](../../notes/general-skills/AWM.md) |
| SkillWeaver | Callable Playwright skills | Practice, execution, and repair | Self-improving web interaction | arXiv preprint; [PDF](../../papers/general-skills/2025/arXiv/SkillWeaver%20-%20Web%20Agents%20can%20Self-Improve%20by%20Discovering%20and%20Honing%20Skills.pdf); [arXiv](https://arxiv.org/abs/2504.07079); [Code](https://github.com/OSU-NLP-Group/SkillWeaver) | [Note](../../notes/general-skills/SkillWeaver.md) |
| XSkill | Task skills + action experiences | Multimodal trajectories | Continual reuse without parameter updates | ICML 2026 (accepted); [PDF](../../papers/general-skills/2026/ICML/XSkill%20-%20Continual%20Learning%20from%20Experience%20and%20Skills%20in%20Multimodal%20Agents.pdf); [arXiv](https://arxiv.org/abs/2603.12056); [Code](https://github.com/XSkill-Agent/XSkill) | [Note](../../notes/general-skills/XSkill.md) |
| Trace2Skill | Portable skill files | Parallel trajectory analysis | Distillation and consolidation | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/Trace2Skill%20-%20Distill%20Trajectory-Local%20Lessons%20into%20Transferable%20Agent%20Skills.pdf); [arXiv](https://arxiv.org/abs/2603.25158); [Code](https://github.com/Qwen-Applications/Trace2Skill) | [Note](../../notes/general-skills/Trace2Skill.md) |
| SkillOpt | Textual skill state | Rollout, reflection, and held-out acceptance | Controlled skill optimization | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/SkillOpt%20-%20Executive%20Strategy%20for%20Self-Evolving%20Agent%20Skills.pdf); [arXiv](https://arxiv.org/abs/2605.23904); [Code](https://github.com/microsoft/SkillOpt) | [Note](../../notes/general-skills/SkillOpt.md) |
| SkillCAT | Hierarchical skill topology | Contrastive successes/failures + replay assessment | Safe skill patching and routing | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/SkillCAT%20-%20Contrastive%2C%20Assessment-Augmented%20and%20Topology-Aware%20Skill%20Self-Evolution%20for%20LLM%20Agents.pdf); [arXiv](https://arxiv.org/abs/2606.13317); Code: not listed | [Note](../../notes/general-skills/SkillCAT.md) |
| EvoSkill | Validated skill frontier | Executor evidence + candidate validation | Iterative skill discovery | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/EvoSkill%20-%20Automated%20Skill%20Discovery%20for%20Multi-Agent%20Systems.pdf); [arXiv](https://arxiv.org/abs/2603.02766); [Code](https://github.com/sentient-agi/EvoSkill) | [Note](../../notes/general-skills/EvoSkill.md) |
| Earth-Agent | Tool-use trajectory | Runtime observations | EO task execution with a frozen LLM backbone | ICLR 2026; [PDF](../../papers/remote-sensing/2026/ICLR/Earth-Agent%20-%20Unlocking%20the%20Full%20Landscape%20of%20Earth%20Observation%20with%20Agents.pdf); [arXiv](https://arxiv.org/abs/2509.23141); [Code](https://github.com/opendatalab/Earth-Agent) | [Note](../../notes/remote-sensing/Earth-Agent.md) |
| GeoEvolver | Contextual tool constraints | Explored successes and attributed failures | Training-free EO improvement | arXiv preprint; [PDF](../../papers/remote-sensing/2026/arXiv/Experience-Driven%20Multi-Agent%20Systems%20Are%20Training-free%20Context-aware%20Earth%20Observers.pdf); [arXiv](https://arxiv.org/abs/2602.02559); Code: not listed | [Note](../../notes/remote-sensing/GeoEvolver.md) |
| GeoForge | Graph, experience, and SOP memories | Safety-gated trajectory distillation | Non-parametric EO evolution | arXiv preprint 2026; [PDF](../../papers/remote-sensing/2026/arXiv/GeoForge%20-%20Non-Parametric%20Self-Evolving%20Agents%20for%20Earth-Observation%20Reasoning.pdf); [arXiv](https://arxiv.org/abs/2608.10494); Code: not listed | [Note](../../notes/remote-sensing/GeoForge.md) |
| RSMeM | Domain knowledge + compact failure memory | Repeated execution and reflection | Knowledge-dense EO memory evolution | ACL 2026; [PDF](../../papers/remote-sensing/2026/ACL/RSMeM%20-%20Knowledge-Enhanced%20Memory%20Evolution%20for%20Remote%20Sensing%20Agents%20with%20Systematic%20Evaluation.pdf); [arXiv](https://arxiv.org/abs/2607.24772); [Code](https://github.com/AI9Stars/RSMeM) | [Note](../../notes/remote-sensing/RSMeM.md) |
| RS-Claw | Hierarchical tool documentation | Active branch exploration | Context-efficient tool discovery | arXiv preprint 2026; [PDF](../../papers/remote-sensing/2026/arXiv/RS-Claw%20-%20Progressive%20Active%20Tool%20Exploration%20via%20Hierarchical%20Skill%20Trees%20for%20Remote%20Sensing%20Agents.pdf); [arXiv](https://arxiv.org/abs/2605.13391); Code: not listed | [Note](../../notes/remote-sensing/RS-Claw.md) |
| OpenEarth-Agent | Generated executable tools | Runtime errors and debugging | Adaptation to unseen EO operations | arXiv preprint 2026; [PDF](../../papers/remote-sensing/2026/arXiv/OpenEarth-Agent%20-%20From%20Tool%20Calling%20to%20Tool%20Creation%20for%20Open-Environment%20Earth%20Observation.pdf); [arXiv](https://arxiv.org/abs/2603.22148); Code: not listed | [Note](../../notes/remote-sensing/OpenEarth-Agent.md) |

## Mechanism decomposition

| Mechanism | Representative papers | Central variable |
| --- | --- | --- |
| Experience-to-text | ExpeL, GeoEvolver, RSMeM | What failure information transfers? |
| Experience-to-workflow | AWM, GeoForge | How should partial order and dependencies be stored? |
| Experience-to-skill | SkillWeaver, Trace2Skill, XSkill, SkillCAT | When is a procedure reusable rather than task-specific? |
| Experience-to-code/tool | Voyager, SkillWeaver, OpenEarth-Agent | How can execution validate generated capabilities? |
| Retrieval and routing | ExpeL, RS-Claw, GeoForge, XSkill | What state should be loaded under a limited context budget? |

## Open research questions

- Separate real learning from extra inference compute, retries, larger context, or hidden human-authored priors.
- Measure negative transfer and memory pollution, not only average improvement.
- Define held-out task, domain, tool, and temporal splits for genuine continual adaptation.
- Compare textual memory, workflow graphs, executable skills, and parameter updates under matched token and tool budgets.
- Study stability: whether later experiences overwrite, contradict, or silently bypass earlier knowledge.

See also [Agent Memory](../agent-memory/README.md), [Self-Evolving Agents](../self-evolving-agents/README.md), and [Agent Skills](../agent-skills/README.md).
