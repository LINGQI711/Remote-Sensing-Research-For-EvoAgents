# Earth-Agent-Pro: Towards Real-World Full-Chain Earth Observation with Agents

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/arXiv/Earth-Agent-Pro%20-%20Towards%20Real-World%20Full-Chain%20Earth%20Observation%20with%20Agents.pdf) · [Source version](https://arxiv.org/abs/2609.12533v1)

**Venue:** arXiv preprint 2026

**Version read:** v1

**Topic:** Open-world, full-chain EO planning and execution

## 1. What problem does it address?

Existing EO-agent benchmarks usually begin with expert-prepared observations or answer choices. This removes data discovery and acquisition from the evaluated workflow, while multiple-choice answers can hide numerical, date, unit, and grounding errors. A real request instead requires the agent to find suitable observations, prepare them, execute dependent computations, and derive an open-ended answer from runtime evidence.

## 2. How does it solve the problem?

Earth-Agent-Pro separates workflow composition from runtime operation grounding in an execution-adaptive Plan-and-Execute framework. Expert-authored skills constrain both planning and tool scope. Workflow-centered structured memory links pending steps to accepted evidence and provenance, so a failed step triggers local correction or repair of only the affected workflow suffix while preserving a valid prefix. Separate LoRA adapters specialize the roles: sequence-level supervised fine-tuning trains the Planner, and node-level GRPO with locally verifiable rewards trains the Executor's tool arguments.

## 3. What experiments were conducted?

- Earth-Bench-Pro converts 248 scientific task cores into 744 matched questions across Instruction Following, Autonomous Planning, and Open-World Execution. It contains 5,295 reference tool calls and 112 tools; the 248 open-world workflows average 7.1 calls and use 84 distinct tools.
- The open-world subset includes 188 Product and Spectrum tasks requiring runtime acquisition and preprocessing, plus 60 RGB tasks whose concrete files must be discovered during execution.
- Experiments compare multiple proprietary and open backbones. Controlled GPT-5 comparisons cover ReAct, AFlow, OpenEarthAgent, and Earth-Agent-Pro, while transfer and modality analyses use the OpenEarthAgent benchmark and TerraScope.
- Ablations isolate expert skills, dynamic workflow repair, workflow-centered memory, Planner SFT, and Executor GRPO. Planning-only and oracle-plan protocols separately test workflow composition and argument grounding.

## 4. What are the conclusions?

On Earth-Bench-OW with a shared GPT-5 backbone, tool set, and skill set, Earth-Agent-Pro reaches 66.13% LLM-as-Judge accuracy, 20.95 percentage points above ReAct, and improves Tools-In-Order by 24.44 points. Joint Planner and Executor tuning raises Qwen3.5-9B LLM-as-Judge accuracy from 38.31% to 50.00%. However, exact workflow and argument grounding remain substantially weaker than tool coverage: the strongest reported Tool-Exact-Match and parameter scores are 71.01% and 32.77%, respectively. Results also vary by modality, and higher accuracy incurs additional execution latency. The v1 paper states that code and datasets will be released soon, so the benchmark is not yet independently reproducible from a public release.

**Reading pointers:** Sections III-VII; Tables I-II, IV, and VIII-X; PDF pages 3-15.
