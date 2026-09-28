# Agent Training and Reinforcement Learning

[Top-level catalog](../../README.md) · [All collections](../README.md)

This page curates **general-domain** methods that train agent policies, controllers, or reward models with demonstrations, supervised fine-tuning, preference objectives, or reinforcement learning. EO/remote-sensing agent training papers remain only in [Remote Sensing Agents](../remote-sensing-agents/README.md).

## Research storyline

There is a useful progression from **teaching general agent behaviors** to **learning from environment interaction**, then to **assigning credit across multi-step trajectories**, and finally to **training specialized controllers for memory and other agent subsystems**. SFT, RL, and frozen-weight test-time adaptation answer different questions; hybrid systems should identify the learned component and update stage rather than simply say “agent learning.”

| Paper | Training target / method | Venue · PDF · arXiv · Code | Reading note |
| --- | --- | --- | --- |
| AgentTuning | Instruction-tunes on curated multi-task interaction trajectories while mixing general instructions to preserve broad language ability | Findings of ACL 2024 · [PDF](https://aclanthology.org/2024.findings-acl.181.pdf) · [arXiv](https://arxiv.org/abs/2310.12823) · [Code](https://github.com/THUDM/AgentTuning) | External paper |
| Recursive Introspection (RISE) | Fine-tunes an agent to inspect and correct its previous reasoning over multiple turns | arXiv preprint 2024 · [PDF](https://arxiv.org/pdf/2407.18219) · [arXiv](https://arxiv.org/abs/2407.18219) · [Code](https://github.com/cmu-mind/RISE) | External paper |
| WebRL | Online RL for web agents; self-evolving curriculum, outcome reward model, and adaptive policy updates | ICLR 2025 · [PDF](https://openreview.net/attachment?id=oVKEAFjEqv&name=pdf) · [arXiv](https://arxiv.org/abs/2411.02337) · [Code](https://github.com/THUDM/WebRL) | External paper |
| WebAgent-R1 | End-to-end multi-turn RL from online web interactions with task-success rewards | EMNLP 2025 · [PDF](https://aclanthology.org/2025.emnlp-main.401.pdf) · [arXiv](https://arxiv.org/abs/2505.16421) · [Code](https://github.com/weizhepei/WebAgent-R1) | External paper |
| Multi-Agent Collaboration via Evolving Orchestration | RL trains an orchestrator to adaptively activate and sequence agents, with compact cyclic reasoning emerging from learning | NeurIPS 2025 · [PDF](https://proceedings.neurips.cc/paper_files/paper/2025/file/f1320d2e2842169c6fc89dcbd80e94d0-Paper-Conference.pdf) · [arXiv](https://arxiv.org/abs/2505.19591) · [Code](https://github.com/OpenBMB/ChatDev/tree/puppeteer) | External paper |
| AgentRL: Scaling Agentic Reinforcement Learning with a Multi-Turn, Multi-Task Framework | Asynchronous multi-turn rollouts, cross-policy sampling, and task-advantage normalization for scalable multi-task agent RL | arXiv preprint 2025 · [PDF](https://arxiv.org/pdf/2510.04206) · [arXiv](https://arxiv.org/abs/2510.04206) · [Code](https://github.com/THUDM/AgentRL) | External paper |
| Agent-R1: Training Powerful LLM Agents with End-to-End Reinforcement Learning | Modular framework that formalizes agent/environment interaction as an RL process and supports end-to-end agent training | arXiv preprint 2025 · [PDF](https://arxiv.org/pdf/2511.14460) · [arXiv](https://arxiv.org/abs/2511.14460) · [Code](https://github.com/AgentR1/Agent-R1) | External paper |
| Agent Lightning | Decouples agent execution from RL training; uses trajectory conversion and hierarchical credit assignment to train existing agents | arXiv preprint 2025 · [PDF](https://arxiv.org/pdf/2508.03680) · [arXiv](https://arxiv.org/abs/2508.03680) · [Code](https://github.com/microsoft/agent-lightning) | External paper |
| Memory-R1 | Outcome-driven RL for a memory manager (ADD/UPDATE/DELETE/NOOP) and a memory-using answer agent | ACL 2026 · [PDF](https://aclanthology.org/2026.acl-long.583.pdf) · [arXiv](https://arxiv.org/abs/2508.19828) · Code: not listed | External paper |
| MemSkill | Learns a controller over memory-operation skills and evolves the skill bank from hard cases | NeurIPS 2026 · [PDF](../../papers/general-skills/2026/arXiv/MemSkill%20-%20Learning%20and%20Evolving%20Memory%20Skills%20for%20Self-Evolving%20Agents.pdf) · [arXiv](https://arxiv.org/abs/2602.02474) · [Code](https://github.com/ViktorAxelsen/MemSkill) | [Note](../../notes/general-skills/MemSkill.md) |
| AgeMem: Agentic Memory | Trains tool-based long-/short-term memory management with progressive RL | ACL 2026 · [PDF](https://aclanthology.org/2026.acl-long.981.pdf) · [arXiv](https://arxiv.org/abs/2601.01885) · Code: not listed | External paper |

## Compare by what is updated

| Learning target | Representative line | Key experimental question |
| --- | --- | --- |
| Base model instruction-following | AgentTuning | Do interaction traces transfer to unseen agent tasks without eroding general capability? |
| Iterative self-correction | RISE | Does fine-tuning enable reliable correction across turns, beyond extra inference compute? |
| Environment-grounded task policy | WebRL, WebAgent-R1, AgentRL, Agent-R1 | How do reward quality, exploration, environment drift, and long-horizon credit assignment affect success? |
| Learned multi-agent controller | Evolving Orchestration | Does RL learn when to delegate and stop, and do gains survive budget-matched single-agent baselines? |
| Training interface / credit assignment | Agent Lightning | Can the same RL machinery train agents with different runtimes and control flows fairly? |
| Memory controller / operations | Memory-R1, MemSkill, AgeMem | Which memory decisions are learned, what supervision/reward is available, and do gains transfer across memory benchmarks? |

## Experimental controls

- Report which module is updated: base policy, planner, tool selector, memory controller, or reward model.
- Distinguish SFT warm starts from online RL and from training-free prompt or memory adaptation.
- Specify reward granularity, verifier access, rollout budget, replay strategy, and environment version.
- Measure generalization to new tasks/tools, retention, reward hacking, latency, and total training cost.
- Compare against compute-matched frozen-weight baselines and report data contamination, model/checkpoint, and reward-model dependencies.

For external-state adaptation under frozen parameters, see [Training-Free Agent Learning](../training-free-agent-learning/README.md).

