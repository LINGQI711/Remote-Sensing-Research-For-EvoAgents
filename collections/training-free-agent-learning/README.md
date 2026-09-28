# Training-Free Agent Learning

[Top-level catalog](../../README.md) · [All collections](../README.md)

This page curates **general-domain** work where an agent improves at inference time or through external state without updating its backbone parameters in the target interaction loop. EO and remote-sensing examples belong only in [Remote Sensing Agents](../remote-sensing-agents/README.md).

## Research storyline

The field progresses from **acting with a fixed prompt** to **learning across attempts**. ReAct makes reasoning/action interleaving explicit; self-refinement and verbal reinforcement add feedback within an attempt; episodic memory and experience extraction preserve lessons across tasks; workflow/skill induction turns them into reusable procedures. These methods can learn at test time while freezing backbone weights, but their gains still depend on extra context, trials, and verification—so fair evaluation must control all three.

| Paper | External learning state / mechanism | Venue · PDF · arXiv · Code | Reading note |
| --- | --- | --- | --- |
| Reflexion | Verbal feedback stored in episodic memory; no weight update | NeurIPS 2023 · [PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/1b44b878bb782e6954cd888628510e90-Paper-Conference.pdf) · [arXiv](https://arxiv.org/abs/2303.11366) · [Code](https://github.com/noahshinn024/reflexion) | External paper |
| ReAct | Alternates reasoning traces and environment/tool actions; establishes a basic inference-time agent loop | ICLR 2023 · [PDF](https://arxiv.org/pdf/2210.03629) · [arXiv](https://arxiv.org/abs/2210.03629) · [Code](https://github.com/ysymyth/ReAct) | External paper |
| Self-Refine | Iterative self-feedback and revision at test time | NeurIPS 2023 · [PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/91edff07232fb1b55a505a9e9f6c0ff3-Paper-Conference.pdf) · [arXiv](https://arxiv.org/abs/2303.17651) · [Code](https://github.com/madaan/self-refine) | External paper |
| Generative Agents | Persistent memory stream, reflection, and retrieval improve continuity in a simulated society | UIST 2023 · [PDF](https://storage.googleapis.com/gweb-research2023-media/pubtools/7070.pdf) · [arXiv](https://arxiv.org/abs/2304.03442) · [Code](https://github.com/joonspk-research/generative_agents) | External paper |
| MemoryBank | Maintains and updates long-term user memory without task-time parameter updates | AAAI 2024 · [PDF](https://ojs.aaai.org/index.php/AAAI/article/download/29946/31654) · [arXiv](https://arxiv.org/abs/2305.10250) · [Code](https://github.com/zhongwanjun/MemoryBank-SiliconFriend) | External paper |
| MemRL | Improves episodic retrieval utility through runtime, non-parametric RL while keeping backbone weights fixed | arXiv preprint 2026 · [PDF](https://arxiv.org/pdf/2601.03192) · [arXiv](https://arxiv.org/abs/2601.03192) · [Code](https://github.com/MemTensor/MemRL) | External paper |
| Just-In-Time Reinforcement Learning (JitRL) | Uses retrieved episodes to estimate action advantages and modulate output logits at test time; derives the update from a KL-constrained policy objective without gradient updates | arXiv preprint 2026 · [PDF](https://arxiv.org/pdf/2601.18510) · [arXiv](https://arxiv.org/abs/2601.18510) · [Code](https://github.com/liushiliushi/JitRL) | External paper |
| Voyager | Executable skill library, automatic curriculum, and self-verification | TMLR 2024 · [PDF](../../papers/general-skills/2024/TMLR/Voyager%20-%20An%20Open-Ended%20Embodied%20Agent%20with%20Large%20Language%20Models.pdf) · [arXiv](https://arxiv.org/abs/2305.16291) · [Code](https://github.com/MineDojo/Voyager) | [Note](../../notes/general-skills/Voyager.md) |
| ExpeL | Extracted insights and successful demonstrations from prior trials | AAAI 2024 · [PDF](../../papers/general-skills/2024/AAAI/ExpeL%20-%20LLM%20Agents%20Are%20Experiential%20Learners.pdf) · [arXiv](https://arxiv.org/abs/2308.10144) · [Code](https://github.com/LeapLabTHU/ExpeL) | [Note](../../notes/general-skills/ExpeL.md) |
| Agent Workflow Memory (AWM) | Induces reusable workflows from offline examples or online successes | ICML 2025 · [PDF](../../papers/general-skills/2025/ICML/Agent%20Workflow%20Memory.pdf) · [arXiv](https://arxiv.org/abs/2409.07429) · [Code](https://github.com/zorazrw/agent-workflow-memory) | [Note](../../notes/general-skills/AWM.md) |
| SkillWeaver | Discovers, implements, practices, and repairs callable web skills | arXiv preprint 2025 · [PDF](../../papers/general-skills/2025/arXiv/SkillWeaver%20-%20Web%20Agents%20can%20Self-Improve%20by%20Discovering%20and%20Honing%20Skills.pdf) · [arXiv](https://arxiv.org/abs/2504.07079) · [Code](https://github.com/OSU-NLP-Group/SkillWeaver) | [Note](../../notes/general-skills/SkillWeaver.md) |
| Trace2Skill | Distills trajectory-local lessons into portable, reusable skills | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/Trace2Skill%20-%20Distill%20Trajectory-Local%20Lessons%20into%20Transferable%20Agent%20Skills.pdf) · [arXiv](https://arxiv.org/abs/2603.25158) · [Code](https://github.com/Qwen-Applications/Trace2Skill) | [Note](../../notes/general-skills/Trace2Skill.md) |
| XSkill | Retrieves and adapts task skills and action-level experience for continual multimodal agents | ICML 2026 · [PDF](../../papers/general-skills/2026/ICML/XSkill%20-%20Continual%20Learning%20from%20Experience%20and%20Skills%20in%20Multimodal%20Agents.pdf) · [arXiv](https://arxiv.org/abs/2603.12056) · [Code](https://github.com/XSkill-Agent/XSkill) | [Note](../../notes/general-skills/XSkill.md) |

## Reading path and boundary with trained adaptation

**ReAct → Self-Refine → Reflexion → ExpeL** moves from action-time reasoning, through same-task critique, to cross-trial episodic lessons. **Voyager → AWM → SkillWeaver → Trace2Skill → XSkill** studies increasingly reusable procedural knowledge. Compare **MemRL** and **JitRL** as two recent test-time RL designs: one learns values for retrieved episodes, the other uses memory-based advantage estimates to adjust action probabilities, both without gradient updates. Ask what persists, what triggers an update, and whether transfer holds on unseen tasks. If a method trains weights or a policy offline, compare it in [Agent Training and RL](../agent-training-rl/README.md); hybrid work should specify exactly what is frozen and what is trained.

## Questions for fair comparisons

- Separate actual external-state learning from extra test-time compute, retries, context, or human-authored priors.
- Match the base model, interaction budget, tool access, and inference tokens against parameter-updated baselines.
- Measure held-out transfer, retention, and negative transfer—not only within-task improvement.
- Compare text memories, workflow graphs, executable skills, and learned policies under the same task stream.

For trained adaptation and RL, see [Agent Training and RL](../agent-training-rl/README.md).

