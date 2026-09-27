# Agent Benchmarks and Evaluation

[Top-level catalog](../../README.md) · [All collections](../README.md)

This page contains **general-domain** agent benchmarks only. Earth-Bench, GeoPlan-Bench, ThinkGeo, and other EO/geospatial benchmarks stay in [Remote Sensing Agents](../remote-sensing-agents/README.md). The benchmarks below cover interactive tool use, web tasks, computer use, memory, and skill utility.

| Benchmark | Primary capability | Venue · PDF · arXiv · Code |
| --- | --- | --- |
| AgentBench | LLM agent reasoning and decision-making across eight interactive environments | ICLR 2024 · [PDF](https://proceedings.iclr.cc/paper_files/paper/2024/file/e9df36b21ff4ee211a8b71ee8b7e9f57-Paper-Conference.pdf) · [arXiv](https://arxiv.org/abs/2308.03688) · [Code](https://github.com/THUDM/AgentBench) |
| GAIA | General assistant ability across reasoning, web browsing, and tool use | ICLR 2024 · [PDF](https://arxiv.org/pdf/2311.12983) · [arXiv](https://arxiv.org/abs/2311.12983) · Code: not listed · [Dataset](https://huggingface.co/gaia-benchmark) |
| WebArena | Long-horizon web tasks on realistic, self-hosted websites | ICLR 2024 · [PDF](https://proceedings.iclr.cc/paper_files/paper/2024/file/4410c0711e9154a7a2d26f9b3816d1ef-Paper-Conference.pdf) · [arXiv](https://arxiv.org/abs/2307.13854) · [Code](https://github.com/webuiagent/webarena-official) |
| OSWorld | Open-ended multimodal computer-use tasks across operating systems and applications | NeurIPS 2024 Datasets & Benchmarks · [PDF](https://proceedings.neurips.cc/paper_files/paper/2024/file/5d413e48f84dc61244b6be550f1cd8f5-Paper-Datasets_and_Benchmarks_Track.pdf) · [arXiv](https://arxiv.org/abs/2404.07972) · [Code](https://github.com/xlang-ai/OSWorld) |
| AndroidWorld | Interactive mobile-device tasks in a reproducible Android environment | ICLR 2025 · [PDF](https://arxiv.org/pdf/2405.14505) · [arXiv](https://arxiv.org/abs/2405.14505) · [Code](https://github.com/google-research/android_world) |
| LongMemEval | Long-term conversational memory and multi-session reasoning | ICLR 2025 · [PDF](https://arxiv.org/pdf/2410.10813) · [arXiv](https://arxiv.org/abs/2410.10813) · [Code](https://github.com/xiaowu0162/LongMemEval) |
| SkillsBench | Whether explicit procedural skills improve performance across diverse tasks | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/SkillsBench%20-%20Benchmarking%20How%20Well%20Agent%20Skills%20Work%20Across%20Diverse%20Tasks.pdf) · [arXiv](https://arxiv.org/abs/2602.12670) · [Code](https://github.com/benchflow-ai/skillsbench) |
| MemoryAgentBench | Memory agents' retrieval, test-time learning, long-range understanding, and conflict resolution | ICLR 2026 · [PDF](https://arxiv.org/pdf/2507.05257) · [arXiv](https://arxiv.org/abs/2507.05257) · [Code](https://github.com/HUST-AI-HYZ/MemoryAgentBench) |

## Evaluation dimensions

| Dimension | Examples | What it diagnoses |
| --- | --- | --- |
| Outcome | Exact match, task completion, execution-based checks | Whether the task was completed correctly |
| Process | Tool choice, arguments, action ordering, recovery | Whether the agent used a reliable trajectory |
| Efficiency | Calls, tokens, latency, cost | Whether the result is operationally practical |
| Transfer | New tasks, tools, environments, temporal splits | Whether capability generalizes |
| Persistent learning | Retention, negative transfer, skill/memory contamination | Whether updates help future tasks safely |

Always report the model, environment version, tool inventory, interaction/retry budget, scoring protocol, and judge configuration. For EO-specific evaluation, use the remote-sensing collection linked above.
