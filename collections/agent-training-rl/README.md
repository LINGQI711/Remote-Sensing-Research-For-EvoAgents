# Agent Training and Reinforcement Learning

[Top-level catalog](../../README.md) · [All collections](../README.md)

This page curates **general-domain** methods that train agent policies, controllers, or reward models with demonstrations, supervised fine-tuning, preference objectives, or reinforcement learning. EO/remote-sensing agent training papers remain only in [Remote Sensing Agents](../remote-sensing-agents/README.md).

| Paper | Training target / method | Venue · PDF · arXiv · Code | Reading note |
| --- | --- | --- | --- |
| WebRL | Online RL for web agents; self-evolving curriculum, outcome reward model, and adaptive policy updates | ICLR 2025 · [PDF](https://openreview.net/attachment?id=oVKEAFjEqv&name=pdf) · [arXiv](https://arxiv.org/abs/2411.02337) · [Code](https://github.com/THUDM/WebRL) | External paper |
| WebAgent-R1 | End-to-end multi-turn RL from online web interactions with task-success rewards | arXiv preprint 2025 · [PDF](https://arxiv.org/pdf/2505.16421) · [arXiv](https://arxiv.org/abs/2505.16421) · Code: not listed | External paper |
| MemSkill | Reinforcement learning over memory-operation choices and a memory-skill controller | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/MemSkill%20-%20Learning%20and%20Evolving%20Memory%20Skills%20for%20Self-Evolving%20Agents.pdf) · [arXiv](https://arxiv.org/abs/2602.02474) · [Code](https://github.com/ViktorAxelsen/MemSkill) | [Note](../../notes/general-skills/MemSkill.md) |
| AgeMem: Agentic Memory | Trains tool-based long-/short-term memory management with progressive RL | ACL 2026 · [PDF](https://aclanthology.org/2026.acl-long.981.pdf) · [arXiv](https://arxiv.org/abs/2601.01885) · Code: not listed | External paper |

## Experimental controls

- Report which module is updated: base policy, planner, tool selector, memory controller, or reward model.
- Distinguish SFT warm starts from online RL and from training-free prompt or memory adaptation.
- Specify reward granularity, verifier access, rollout budget, replay strategy, and environment version.
- Measure generalization to new tasks/tools, retention, reward hacking, latency, and total training cost.

For external-state adaptation under frozen parameters, see [Training-Free Agent Learning](../training-free-agent-learning/README.md).
