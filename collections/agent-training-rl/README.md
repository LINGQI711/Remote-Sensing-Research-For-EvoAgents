# Agent Training and Reinforcement Learning

[Top-level catalog](../../README.md) · [All collections](../README.md)

This collection covers parameter-updating approaches for agent behavior. It separates planner training, executor/tool grounding, controller learning, and end-to-end agentic MLLM training because these objectives produce different capabilities and failure modes.

## Trained agent mechanisms

| Paper | Trained component | Objective/data | Main evaluation | Venue / PDF / arXiv / Code | Reading note |
| --- | --- | --- | --- | --- | --- |
| OpenEarthAgent | Compact geospatial language model | Response-only SFT over 14,538 validated tool trajectories | Tool arguments, sequence match, and end-to-end answers | arXiv preprint; [PDF](../../papers/remote-sensing/2026/arXiv/OpenEarthAgent%20-%20A%20Unified%20Framework%20for%20Tool-Augmented%20Geospatial%20Agents.pdf); [arXiv](https://arxiv.org/abs/2602.17665); [Code](https://github.com/mbzuai-oryx/OpenEarthAgent) | [Note](../../notes/remote-sensing/OpenEarthAgent.md) |
| RemoteAgent | Agentic multimodal model | Reinforcement learning for vague-intent resolution | Intent accuracy and downstream RS tasks | arXiv preprint; [PDF](../../papers/remote-sensing/2026/arXiv/RemoteAgent%20-%20Bridging%20Vague%20Human%20Intents%20and%20Earth%20Observation%20with%20RL-based%20Agentic%20MLLMs.pdf); [arXiv](https://arxiv.org/abs/2604.07765); [Code](https://github.com/1e12Leon/RemoteAgent) | [Note](../../notes/remote-sensing/RemoteAgent.md) |
| HiRS-Agent | Shared manager/specialist backbone | Expert tuning + verification-guided hierarchical GRPO/LoRA | Earth-Bench, ThinkGeo, expertise and retention | ACM Multimedia 2026 (accepted); [PDF](../../papers/remote-sensing/2026/ACM-MM/HiRS-Agent%20-%20A%20Hierarchical%20Multi-Agent%20System%20for%20Reliable%20Long-Horizon%20Remote%20Sensing%20Task%20Solving.pdf); [arXiv](https://arxiv.org/abs/2608.30672); Code: not listed | [Note](../../notes/remote-sensing/HiRS-Agent.md) |
| Earth-Agent-Pro | Separate Planner and Executor adapters | Planner SFT + node-level Executor GRPO with local rewards | Earth-Bench-Pro planning, execution, and open-world answers | arXiv preprint 2026; [PDF](../../papers/remote-sensing/2026/arXiv/Earth-Agent-Pro%20-%20Towards%20Real-World%20Full-Chain%20Earth%20Observation%20with%20Agents.pdf); [arXiv](https://arxiv.org/abs/2609.12533); Code: not listed | [Note](../../notes/remote-sensing/Earth-Agent-Pro.md) |
| MemSkill | Memory-skill controller | Reinforcement learning over memory-operation choices | Memory-use effectiveness and evolving inventory | arXiv preprint; [PDF](../../papers/general-skills/2026/arXiv/MemSkill%20-%20Learning%20and%20Evolving%20Memory%20Skills%20for%20Self-Evolving%20Agents.pdf); [arXiv](https://arxiv.org/abs/2602.02474); [Code](https://github.com/ViktorAxelsen/MemSkill) | [Note](../../notes/general-skills/MemSkill.md) |
| GeoAgent | Geolocation model | Reinforcement with spatial, semantic, and consistency rewards | Visual geolocation | CVPR 2026; [PDF](../../papers/remote-sensing/2026/CVPR/GeoAgent%20-%20Learning%20to%20Geolocate%20Everywhere%20with%20Reinforced%20Geographic%20Characteristics.pdf); [arXiv](https://arxiv.org/abs/2602.12617); [Code](https://github.com/HVision-NKU/GeoAgent) | [Note](../../notes/remote-sensing/GeoAgent.md) |

## Research axes

| Axis | Questions to control experimentally |
| --- | --- |
| Training target | Planner, tool selector, argument generator, verifier, memory controller, or full policy? |
| Supervision | Demonstration, execution trace, verifier reward, preference, final outcome, or process reward? |
| Credit assignment | Task-level return, step-level reward, node-local reward, or hierarchical objectives? |
| Environment | Static tool schemas or changing tools, observations, and failure states? |
| Generalization | New tasks, tools, domains, modalities, workflow lengths, and user intent ambiguity? |
| Retention | Does specialization damage general reasoning, instruction following, or prior skills? |

## Training-free versus trained adaptation

Matched comparisons should hold the backbone, tool environment, experience budget, retries, and inference tokens constant. Parameter updates may improve compact-model reliability, while external memory and skills can update faster and remain inspectable. Hybrid systems such as Earth-Agent-Pro make the comparison especially important because trained adapters and expert-authored skills contribute jointly.

## Research gaps

- Fair process-reward design when only some tool outputs are locally verifiable.
- Offline-to-online mismatch in tool trajectories and environment failures.
- Continual RL without catastrophic forgetting or reward hacking.
- Training compact agents that retain calibrated stopping and rejection behavior.
- Joint optimization of quality, latency, token cost, and tool cost.

See also [Training-Free Agent Learning](../training-free-agent-learning/README.md) for external-state alternatives.
