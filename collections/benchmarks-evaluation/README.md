# Agent Benchmarks and Evaluation

[Top-level catalog](../../README.md) · [All collections](../README.md)

This collection separates outcome quality from the mechanisms that produce it. Agent evaluation should cover final answers, trajectories, tool and argument correctness, efficiency, recovery, transfer, and the validity of persistent updates.

## Benchmarks in and around the library

| Benchmark | Primary capability | Scale / protocol | Venue / PDF / arXiv / Code | Local paper or source |
| --- | --- | --- | --- | --- |
| Earth-Bench | Cross-modal EO tool execution over RGB, spectra, and products | 248 questions, 13,729 images, 1,345 steps, 104 tools; AP and IF | ICLR 2026; [PDF](../../papers/remote-sensing/2026/ICLR/Earth-Agent%20-%20Unlocking%20the%20Full%20Landscape%20of%20Earth%20Observation%20with%20Agents.pdf); [arXiv](https://arxiv.org/abs/2509.23141); [Code](https://github.com/opendatalab/Earth-Agent) | [Earth-Agent note](../../notes/remote-sensing/Earth-Agent.md) |
| Earth-Bench-Pro | Matched IF, AP, and open-world execution | 248 task cores -> 744 questions, 5,295 calls, 112 tools | arXiv preprint 2026; [PDF](../../papers/remote-sensing/2026/arXiv/Earth-Agent-Pro%20-%20Towards%20Real-World%20Full-Chain%20Earth%20Observation%20with%20Agents.pdf); [arXiv](https://arxiv.org/abs/2609.12533); Code: not listed | [Earth-Agent-Pro note](../../notes/remote-sensing/Earth-Agent-Pro.md) |
| ThinkGeo | Step-level remote-sensing tool-use diagnosis | 486 optical/SAR tasks and 1,778 expert-verified steps | arXiv preprint; [PDF](../../papers/remote-sensing/2025/arXiv/ThinkGeo%20-%20Evaluating%20Tool-Augmented%20Agents%20for%20Remote%20Sensing%20Tasks.pdf); [arXiv](https://arxiv.org/abs/2505.23752); [Code](https://github.com/mbzuai-oryx/ThinkGeo) | [ThinkGeo note](../../notes/remote-sensing/ThinkGeo.md) |
| UnivEARTH | Evidence-grounded EO coding with Google Earth Engine | 408 yes/no questions in the ACL 2026 version | Findings of ACL 2026; [PDF](../../papers/remote-sensing/2026/ACL-Findings/Towards%20LLM%20Agents%20for%20Earth%20Observation.pdf); [arXiv](https://arxiv.org/abs/2504.12110); Code: not listed | [UnivEARTH note](../../notes/remote-sensing/UnivEARTH.md) |
| GeoMMBench | Expert multimodal geoscience and RS reasoning | 36 models plus human participants | CVPR 2026 (Highlight); [PDF](../../papers/remote-sensing/2026/CVPR/GeoMMBench%20and%20GeoMMAgent%20-%20Toward%20Expert-Level%20Multimodal%20Intelligence%20in%20Geoscience%20and%20Remote%20Sensing.pdf); [arXiv](https://arxiv.org/abs/2604.08896); [Code](https://github.com/Shihao-Cheng/GeoMMAgent) | [GeoMMAgent note](../../notes/remote-sensing/GeoMMAgent.md) |
| OpenEarth-Bench | Open-environment EO tool creation | 596 full-pipeline cases across seven domains | arXiv preprint 2026; [PDF](../../papers/remote-sensing/2026/arXiv/OpenEarth-Agent%20-%20From%20Tool%20Calling%20to%20Tool%20Creation%20for%20Open-Environment%20Earth%20Observation.pdf); [arXiv](https://arxiv.org/abs/2603.22148); Code: not listed | [OpenEarth-Agent note](../../notes/remote-sensing/OpenEarth-Agent.md) |
| OpenEarthAgent evaluation | Compact geospatial tool-agent training and transfer | 1,169 evaluation examples with live-tool and stepwise protocols | arXiv preprint; [PDF](../../papers/remote-sensing/2026/arXiv/OpenEarthAgent%20-%20A%20Unified%20Framework%20for%20Tool-Augmented%20Geospatial%20Agents.pdf); [arXiv](https://arxiv.org/abs/2602.17665); [Code](https://github.com/mbzuai-oryx/OpenEarthAgent) | [OpenEarthAgent note](../../notes/remote-sensing/OpenEarthAgent.md) |
| REMSA benchmark | Constraint-aware RS foundation-model recommendation | Expert-scored model suitability rather than downstream adapted accuracy | arXiv preprint; [PDF](../../papers/remote-sensing/2025/arXiv/REMSA%20-%20Foundation%20Model%20Selection%20for%20Remote%20Sensing%20via%20a%20Constraint-Aware%20Agent.pdf); [arXiv](https://arxiv.org/abs/2511.17442); [Code](https://github.com/be-chen/REMSA) | [REMSA note](../../notes/remote-sensing/REMSA.md) |
| GeoLLM-Engine | Executable geospatial copilot environment | More than 175 tools and formal state | CVPR 2024 Workshops · EarthVision; [PDF](../../papers/remote-sensing/2024/CVPR-Workshops/GeoLLM-Engine%20-%20A%20Realistic%20Environment%20for%20Building%20Geospatial%20Copilots.pdf); [arXiv](https://arxiv.org/abs/2404.15500); Code: not listed | [GeoLLM-Engine note](../../notes/remote-sensing/GeoLLM-Engine.md) |
| GeoLLM-QA | State-dependent platform interaction | 1,000 tasks with oracle detections | ICLR 2024 Workshops · ML4RS; [PDF](../../papers/remote-sensing/2024/ICLR-Workshops/Evaluating%20Tool-Augmented%20Agents%20in%20Remote%20Sensing%20Platforms.pdf); [arXiv](https://arxiv.org/abs/2405.00709); Code: not listed | [GeoLLM-QA note](../../notes/remote-sensing/GeoLLM-QA.md) |
| SkillsBench | Effectiveness of agent skills across expertise-heavy tasks | Task-skill pairs with deterministic verifiers | arXiv preprint 2026; [PDF](../../papers/general-skills/2026/arXiv/SkillsBench%20-%20Benchmarking%20How%20Well%20Agent%20Skills%20Work%20Across%20Diverse%20Tasks.pdf); [arXiv](https://arxiv.org/abs/2602.12670); [Code](https://github.com/benchflow-ai/skillsbench) | [SkillsBench note](../../notes/general-skills/SkillsBench.md) |
| GeoPlan-Bench | Long-horizon geospatial workflow planning | Paper reports 1,244 validated tasks; later work may use a 996-task split | [arXiv](https://arxiv.org/abs/2511.17198) · [Code](https://github.com/earth-insights/GeoPlan-bench) |
| TerraBench | Heterogeneous Earth-system reasoning | 403 tasks and about 24,500 verified execution steps | [arXiv](https://arxiv.org/abs/2606.13148) |
| GeoNatureAgent Benchmark | Tool calling against an environmental geospatial API | 93 tasks, 18 categories, 16 tools | [arXiv](https://arxiv.org/abs/2606.12821) |

## Cross-benchmark EO agents

| Agent | Benchmarks | Representative reported evidence | Caution |
| --- | --- | --- | --- |
| Earth-Agent | Earth-Bench | GPT-5 final accuracy 65.99 AP / 62.35 IF in archived v3 | Version- and setting-specific |
| Earth-Agent-Pro | Earth-Bench-Pro | GPT-5 LLM-as-Judge 66.13% on OW; +20.95 points over ReAct | Open-ended LLM-judge metric; v1 preprint |
| GeoEvolver | Earth-Agent task set, ThinkGeo, GeoPlan-Bench | GeoPlan F1_key 0.63; ThinkGeo answer accuracy 46.88 | Earth task set and benchmark splits must be matched |
| OpenEarth-Agent | OpenEarth-Bench, Earth-Bench | GPT-5 Earth-Bench 59.92% with six tools and 67.61% with full tools | Tool inventory changes the comparison |
| RS-Claw | Earth-Bench subset | Qwen3-32B AP +12.45 points over Flat; about 86% fewer input tokens | Uses 234 questions after exclusions |
| HiRS-Agent | Earth-Bench, ThinkGeo | Qwen3-4B reaches 43.95/45.56 AP/IF after training | Includes parameter training |
| RSMeM | Earth-Bench | DeepSeek-V3.2 R@3 reaches 57.89% vs 51.82% baseline | Repeated-attempt protocol |
| GeoForge | Earth-Bench, ThinkGeo, GeoPlan-Bench | GPT-5 Earth-Bench 74.33%; GeoPlan F1_key 0.77 | Preprint and protocol-specific |

## Metric layers

| Layer | Example metrics | What it reveals |
| --- | --- | --- |
| Outcome | Exact match, accuracy, LLM judge, numeric tolerance | Whether the final result is acceptable |
| Tool set | Any-order coverage, key-tool recall/precision | Whether necessary operations were selected |
| Ordering | In-order score, exact sequence, edit distance | Whether dependencies were respected |
| Arguments | Exact/structured parameter match | Whether tools were grounded correctly |
| Execution | Success, recovery, retries, valid artifacts | Whether the workflow actually ran |
| Efficiency | Calls, tokens, latency, cost | Whether improvement is operationally practical |
| Learning | Forward transfer, retention, negative transfer | Whether memory/skills improve later tasks safely |

## Comparison cautions

- Earth-Agent, Earth-Agent-Pro, EarthAgent/HTAM, OpenEarth-Agent, and OpenEarthAgent are distinct systems.
- Full vs Lite, AP vs IF vs OW, 248 vs 234 questions, unavailable tools, and R@1 vs R@3 are not interchangeable.
- GeoPlan-Bench task counts and splits differ across versions and follow-up papers.
- Final accuracy, tool coverage, argument accuracy, structural similarity, and Elo-style completeness should not be averaged into a single score.
- LLM-as-judge results need judge identity, prompts, sampling, and agreement checks.

For mechanism-specific evaluation, continue to [Agent Memory](../agent-memory/README.md), [Agent Skills](../agent-skills/README.md), and [Self-Evolving Agents](../self-evolving-agents/README.md).
