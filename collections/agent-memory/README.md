# Agent Memory

[Top-level catalog](../../README.md) · [All collections](../README.md)

This collection is restricted to **general-domain agent memory research**. Remote-sensing and EO papers are indexed only in [Remote Sensing Agents](../remote-sensing-agents/README.md). The papers below cover memory architectures, learning/evolution of memory operations, and memory-specific evaluation.

## Memory mechanisms

| Paper | Mechanism / evidence | Venue · PDF · arXiv · Code | Reading note |
| --- | --- | --- | --- |
| ExpeL | Extracts reusable insights and demonstrations from successes and failures | AAAI 2024 · [PDF](../../papers/general-skills/2024/AAAI/ExpeL%20-%20LLM%20Agents%20Are%20Experiential%20Learners.pdf) · [arXiv](https://arxiv.org/abs/2308.10144) · [Code](https://github.com/LeapLabTHU/ExpeL) | [Note](../../notes/general-skills/ExpeL.md) |
| MemGPT | Hierarchical context management with explicit archival memory | arXiv preprint · [PDF](https://arxiv.org/pdf/2310.08560) · [arXiv](https://arxiv.org/abs/2310.08560) · [Code](https://github.com/cpacker/MemGPT) | External paper |
| Agent Workflow Memory (AWM) | Induces reusable workflows from demonstrations or online successes | ICML 2025 · [PDF](https://arxiv.org/pdf/2409.07429) · [arXiv](https://arxiv.org/abs/2409.07429) · [Code](https://github.com/zorazrw/agent-workflow-memory) | [Note](../../notes/general-skills/AWM.md) |
| A-MEM | Agent-managed, dynamically linked and evolving memory notes | NeurIPS 2025 · [PDF](https://papers.neurips.cc/paper_files/paper/2025/file/19909c36f51abc4856b4560aff3d36d6-Paper-Conference.pdf) · [arXiv](https://arxiv.org/abs/2502.12110) · [System code](https://github.com/agiresearch/A-mem) | External paper |
| MemSkill | Models memory operations as skills and learns a controller to select them | arXiv preprint 2026 · [PDF](https://arxiv.org/pdf/2602.02474) · [arXiv](https://arxiv.org/abs/2602.02474) · [Code](https://github.com/ViktorAxelsen/MemSkill) | [Note](../../notes/general-skills/MemSkill.md) |
| XSkill | Continual multimodal agent learning from task skills and action experiences | ICML 2026 · [PDF](https://arxiv.org/pdf/2603.12056) · [arXiv](https://arxiv.org/abs/2603.12056) · [Code](https://github.com/XSkill-Agent/XSkill) | [Note](../../notes/general-skills/XSkill.md) |

## Memory benchmarks

| Benchmark | What it measures | Venue · PDF · arXiv · Code |
| --- | --- | --- | --- |
| LongMemEval | Long-term conversational memory: extraction, multi-session and temporal reasoning, knowledge updates, abstention | ICLR 2025 · [PDF](https://arxiv.org/pdf/2410.10813) · [arXiv](https://arxiv.org/abs/2410.10813) · [Code](https://github.com/xiaowu0162/LongMemEval) |
| MemoryAgentBench | Incremental multi-turn memory: accurate retrieval, test-time learning, long-range understanding, conflict resolution | ICLR 2026 · [PDF](https://arxiv.org/pdf/2507.05257) · [arXiv](https://arxiv.org/abs/2507.05257) · [Code](https://github.com/HUST-AI-HYZ/MemoryAgentBench) |

## Comparison axes

| Axis | Alternatives to compare |
| --- | --- |
| Representation | Text lessons, demonstrations, key-value records, workflow graphs, executable programs, multimodal traces |
| Write policy | Every trajectory, successes only, failures only, contrastive pairs, verifier-gated updates |
| Retrieval | Similarity, topology, task type, tool constraints, uncertainty, learned controller |
| Maintenance | Append, merge, compress, revise, decay, forget, resolve conflicts |
| Evaluation | Retrieval accuracy, future-task gain, retention, negative transfer, token cost, contamination resistance |

See also [Training-Free Agent Learning](../training-free-agent-learning/README.md), [Self-Evolving Agents](../self-evolving-agents/README.md), and [Benchmarks and Evaluation](../benchmarks-evaluation/README.md).
