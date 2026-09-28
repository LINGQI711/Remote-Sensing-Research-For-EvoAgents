# Agent Benchmarks and Evaluation

[Top-level catalog](../../README.md) · [All collections](../README.md)

This page contains **general-domain** agent benchmarks only. Earth-Bench, GeoPlan-Bench, ThinkGeo, and other EO/geospatial benchmarks stay in [Remote Sensing Agents](../remote-sensing-agents/README.md). The benchmarks below cover interactive tool use, web tasks, computer use, memory, and skill utility.

## How the evaluation landscape fits together

No single score captures agent capability. A useful map runs from broad **multi-environment competence**, through **goal completion in interactive web/computer environments**, to **reliability under user policies**, then to cross-task **persistent learning** (memory/skills). Benchmarks also differ in what is judged: final answer, resulting environment state, action trajectory, or future-task improvement. Always compare results only under matching task splits, model, tools, retries, judge, and budget.

| Benchmark | Primary capability | Venue · PDF · arXiv · Code |
| --- | --- | --- |
| AgentBench | LLM agent reasoning and decision-making across eight interactive environments | ICLR 2024 · [PDF](https://proceedings.iclr.cc/paper_files/paper/2024/file/e9df36b21ff4ee211a8b71ee8b7e9f57-Paper-Conference.pdf) · [arXiv](https://arxiv.org/abs/2308.03688) · [Code](https://github.com/THUDM/AgentBench) |
| GAIA | General assistant ability across reasoning, web browsing, and tool use | ICLR 2024 · [PDF](https://arxiv.org/pdf/2311.12983) · [arXiv](https://arxiv.org/abs/2311.12983) · Code: not listed · [Dataset](https://huggingface.co/gaia-benchmark) |
| WebArena | Long-horizon web tasks on realistic, self-hosted websites | ICLR 2024 · [PDF](https://proceedings.iclr.cc/paper_files/paper/2024/file/4410c0711e9154a7a2d26f9b3816d1ef-Paper-Conference.pdf) · [arXiv](https://arxiv.org/abs/2307.13854) · [Code](https://github.com/webuiagent/webarena-official) |
| OSWorld | Open-ended multimodal computer-use tasks across operating systems and applications | NeurIPS 2024 Datasets & Benchmarks · [PDF](https://proceedings.neurips.cc/paper_files/paper/2024/file/5d413e48f84dc61244b6be550f1cd8f5-Paper-Datasets_and_Benchmarks_Track.pdf) · [arXiv](https://arxiv.org/abs/2404.07972) · [Code](https://github.com/xlang-ai/OSWorld) |
| AndroidWorld | Interactive mobile-device tasks in a reproducible Android environment | ICLR 2025 · [PDF](https://arxiv.org/pdf/2405.14505) · [arXiv](https://arxiv.org/abs/2405.14505) · [Code](https://github.com/google-research/android_world) |
| MultiAgentBench | Evaluates multi-agent collaboration across task completion, collaboration quality, and role specialization in multiple scenarios | ACL 2025 · [PDF](https://aclanthology.org/2025.acl-long.421.pdf) · [arXiv](https://arxiv.org/abs/2503.01935) · [Code](https://github.com/ulab-uiuc/MARBLE) |
| τ-bench | Multi-turn tool-agent-user interactions under domain policies; includes repeated-trial reliability via pass^k | arXiv preprint 2024 · [PDF](https://arxiv.org/pdf/2406.12045) · [arXiv](https://arxiv.org/abs/2406.12045) · [Code](https://github.com/sierra-research/tau-bench) |
| LongMemEval | Long-term conversational memory and multi-session reasoning | ICLR 2025 · [PDF](https://arxiv.org/pdf/2410.10813) · [arXiv](https://arxiv.org/abs/2410.10813) · [Code](https://github.com/xiaowu0162/LongMemEval) |
| MemBench | Memory effectiveness, efficiency, and capacity over multi-faceted memory tasks | Findings of ACL 2025 · [PDF](https://aclanthology.org/2025.findings-acl.989.pdf) · [arXiv](https://arxiv.org/abs/2506.21605) · [Code](https://github.com/import-myself/Membench) |
| SkillsBench | Whether explicit procedural skills improve performance across diverse tasks | arXiv preprint 2026 · [PDF](../../papers/general-skills/2026/arXiv/SkillsBench%20-%20Benchmarking%20How%20Well%20Agent%20Skills%20Work%20Across%20Diverse%20Tasks.pdf) · [arXiv](https://arxiv.org/abs/2602.12670) · [Code](https://github.com/benchflow-ai/skillsbench) |
| MemoryAgentBench | Four memory competencies: accurate retrieval, test-time learning, long-range understanding, and selective forgetting | ICLR 2026 · [PDF](https://arxiv.org/pdf/2507.05257) · [arXiv](https://arxiv.org/abs/2507.05257) · [Code](https://github.com/HUST-AI-HYZ/MemoryAgentBench) |
| MemoryArena | Interdependent multi-session tasks link agent memory with later action in web navigation, planning, search, and reasoning environments | ICML 2026 · [PDF](https://arxiv.org/pdf/2602.16313) · [arXiv](https://arxiv.org/abs/2602.16313) · [Code](https://github.com/ZexueHe/MemoryArena) |
| AMA-Bench | Long-context retention and long-horizon memory built from agent trajectories, with variable task horizons | ICML 2026 · [PDF](https://arxiv.org/pdf/2602.22769) · [arXiv](https://arxiv.org/abs/2602.22769) · [Code](https://github.com/AMA-Bench/AMA-Bench) |
| Mem2ActBench | Whether long-term memory informs actual tool selection and argument grounding in persistent-assistant tasks | ACL 2026 · [PDF](https://aclanthology.org/2026.acl-long.370.pdf) · [arXiv](https://arxiv.org/abs/2601.19935) · [Code](https://github.com/Cantaloupe-M/Mem2ActBench) |
| AMemGym | On-policy personalized-memory evaluation in interactive, evolving user/task environments | ICLR 2026 · [PDF](https://arxiv.org/pdf/2603.01966) · [arXiv](https://arxiv.org/abs/2603.01966) · [Project / code](https://agi-eval-official.github.io/amemgym/) |
| AgentWebBench | Decentralized multi-agent coordination on web tasks, including communication and decentralized planning | arXiv preprint 2026 · [PDF](https://arxiv.org/pdf/2604.10938) · [arXiv](https://arxiv.org/abs/2604.10938) · [Code](https://github.com/cxcscmu/AgentWebBench) |
| Silo-Bench | Scalable benchmark for distributed agent coordination and collaboration under siloed information | arXiv preprint 2026 · [PDF](https://arxiv.org/pdf/2603.01045) · [arXiv](https://arxiv.org/abs/2603.01045) · Code: not listed |
| SkillFlow | Lifelong skill discovery and evolution across 166 sequential tasks in 20 task families; evaluates skill creation, repair, transfer, and library maintenance | arXiv preprint 2026 · [PDF](https://arxiv.org/pdf/2604.17308) · [arXiv](https://arxiv.org/abs/2604.17308) · [Project page](https://zhangzi-a.github.io/SkillFlow-project-page/) |
| SkillEvolBench | Separates reusable skill formation from trajectory memorization in continual skill-learning evaluation | arXiv preprint 2026 · [PDF](https://arxiv.org/pdf/2605.24117) · [arXiv](https://arxiv.org/abs/2605.24117) · [Project page](https://skillevolbench.github.io/) |

For a mechanism-oriented reading path, use **AgentBench / GAIA** as broad task suites, **WebArena / OSWorld / AndroidWorld / τ-bench** for environment-specific interaction and reliability, and **MultiAgentBench / AgentWebBench / Silo-Bench** for collaboration. For persistent learning, compare **LongMemEval / MemBench / MemoryAgentBench / MemoryArena / AMA-Bench / Mem2ActBench / AMemGym**; **SkillsBench / SkillFlow / SkillEvolBench** test whether reusable procedures help, transfer, and improve over a sequence of tasks.

## Evaluation dimensions

| Dimension | Examples | What it diagnoses |
| --- | --- | --- |
| Outcome | Exact match, task completion, execution-based checks | Whether the task was completed correctly |
| Process | Tool choice, arguments, action ordering, recovery | Whether the agent used a reliable trajectory |
| Efficiency | Calls, tokens, latency, cost | Whether the result is operationally practical |
| Transfer | New tasks, tools, environments, temporal splits | Whether capability generalizes |
| Persistent learning | Retention, negative transfer, skill/memory contamination | Whether updates help future tasks safely |

Always report the model, environment version, tool inventory, interaction/retry budget, scoring protocol, and judge configuration. For EO-specific evaluation, use the remote-sensing collection linked above.

