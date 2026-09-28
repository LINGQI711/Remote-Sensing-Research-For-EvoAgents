# Agent Memory

[Top-level catalog](../../README.md) · [All collections](../README.md)

This collection curates **general-domain agent memory**: how interaction history becomes persistent state, how that state is organized and maintained, how agents learn memory operations, and how memory should be evaluated. Remote-sensing and EO work is indexed only in [Remote Sensing Agents](../remote-sensing-agents/README.md).

## Research storyline

Memory research is not just “put old chats in a vector database.” A useful progression is:

1. **Why memory?** Context windows are finite, and long-running agents must preserve relevant experience, user facts, plans, and unresolved state across tasks.
2. **What is stored?** Raw episodes, reflections, profiles/facts, procedural workflows, or linked notes encode different kinds of knowledge.
3. **How is it maintained?** The agent must decide what to write, retrieve, revise, merge, compress, or forget—and when.
4. **Who controls these operations?** Early systems use fixed heuristics; newer work learns memory policies or makes the memory itself an evolving skill.
5. **How do we know it helps?** Evaluation is moving from isolated recall questions to incremental, multi-session tasks where memory changes future decisions and outcomes.

## A. Foundations: from experience streams to persistent context

| Paper | Contribution / memory model | Venue · PDF · arXiv · Code | Reading note |
| --- | --- | --- | --- |
| Generative Agents: Interactive Simulacra of Human Behavior | Memory stream plus relevance/recency/importance retrieval and higher-level reflections; an influential agent-memory design pattern | UIST 2023 · [PDF](https://storage.googleapis.com/gweb-research2023-media/pubtools/7070.pdf) · [arXiv](https://arxiv.org/abs/2304.03442) · [Code](https://github.com/joonspk-research/generative_agents) | External paper |
| Reflexion | Stores verbal self-critique as episodic feedback to guide subsequent attempts without updating model weights | NeurIPS 2023 · [PDF](https://proceedings.neurips.cc/paper_files/paper/2023/file/1b44b878bb782e6954cd888628510e90-Paper-Conference.pdf) · [arXiv](https://arxiv.org/abs/2303.11366) · [Code](https://github.com/noahshinn024/reflexion) | External paper |
| MemGPT | Treats context as a hierarchy: working context is managed against external archival memory through explicit control operations | arXiv preprint 2023 · [PDF](https://arxiv.org/pdf/2310.08560) · [arXiv](https://arxiv.org/abs/2310.08560) · [Code](https://github.com/cpacker/MemGPT) | External paper |
| MemoryBank: Enhancing Large Language Models with Long-Term Memory | Persistent user memory with updating and forgetting inspired by human memory decay and recall | AAAI 2024 · [PDF](https://ojs.aaai.org/index.php/AAAI/article/download/29946/31654) · [arXiv](https://arxiv.org/abs/2305.10250) · [Code](https://github.com/zhongwanjun/MemoryBank-SiliconFriend) | External paper |
| ExpeL: LLM Agents Are Experiential Learners | Converts successes and failures into reusable insights and demonstrations that can be retrieved for future tasks | AAAI 2024 · [PDF](../../papers/general-skills/2024/AAAI/ExpeL%20-%20LLM%20Agents%20Are%20Experiential%20Learners.pdf) · [arXiv](https://arxiv.org/abs/2308.10144) · [Code](https://github.com/LeapLabTHU/ExpeL) | [Note](../../notes/general-skills/ExpeL.md) |

## B. Representation and organization: from records to procedures and graphs

| Paper | What becomes memory | Venue · PDF · arXiv · Code | Reading note |
| --- | --- | --- | --- |
| Agent Workflow Memory (AWM) | Induces reusable, executable procedural workflows from demonstrations or online task successes | ICML 2025 · [PDF](../../papers/general-skills/2025/ICML/Agent%20Workflow%20Memory.pdf) · [arXiv](https://arxiv.org/abs/2409.07429) · [Code](https://github.com/zorazrw/agent-workflow-memory) | [Note](../../notes/general-skills/AWM.md) |
| A-MEM | Uses Zettelkasten-inspired notes, dynamic links, and contextual updates so memory structure can evolve as new events arrive | NeurIPS 2025 · [PDF](https://papers.neurips.cc/paper_files/paper/2025/file/19909c36f51abc4856b4560aff3d36d6-Paper-Conference.pdf) · [arXiv](https://arxiv.org/abs/2502.12110) · [System code](https://github.com/agiresearch/A-mem) · [Evaluation code](https://github.com/WujiangXu/AgenticMemory) | External paper |
| Mem0 | Practical persistent conversational memory with extraction, consolidation, and retrieval; explores graph memory as an option | arXiv preprint 2025 · [PDF](https://arxiv.org/pdf/2504.19413) · [arXiv](https://arxiv.org/abs/2504.19413) · [Code](https://github.com/mem0ai/mem0) | External paper |
| XSkill | Stores multimodal task skills and action-level experience for retrieval and continual transfer across tasks | ICML 2026 · [PDF](../../papers/general-skills/2026/ICML/XSkill%20-%20Continual%20Learning%20from%20Experience%20and%20Skills%20in%20Multimodal%20Agents.pdf) · [arXiv](https://arxiv.org/abs/2603.12056) · [Code](https://github.com/XSkill-Agent/XSkill) | [Note](../../notes/general-skills/XSkill.md) |

## C. Learning the memory policy: deciding what to do with memory

This is the key transition from a memory **store** to a memory **manager**. The control problem includes write/skip, retrieve, update/merge, delete/forget, and short-term/long-term transfer.

| Paper | Learned or agentic memory control | Venue · PDF · arXiv · Code | Reading note |
| --- | --- | --- | --- |
| Memory-R1 | RL trains a Memory Manager to choose ADD/UPDATE/DELETE/NOOP and an Answer Agent to select and use relevant entries | ACL 2026 · [PDF](https://aclanthology.org/2026.acl-long.583.pdf) · [arXiv](https://arxiv.org/abs/2508.19828) · Code: not listed | External paper |
| MemRL | Runtime, non-parametric RL updates utility estimates over episodic experience; separates stable reasoning weights from plastic memory | arXiv preprint 2026 · [PDF](https://arxiv.org/pdf/2601.03192) · [arXiv](https://arxiv.org/abs/2601.03192) · [Code](https://github.com/MemTensor/MemRL) | External paper |
| MemSkill | Represents memory operations as reusable skills and trains a controller to select/evolve them | NeurIPS 2026 · [PDF](https://arxiv.org/pdf/2602.02474) · [arXiv](https://arxiv.org/abs/2602.02474) · [Code](https://github.com/ViktorAxelsen/MemSkill) | [Note](../../notes/general-skills/MemSkill.md) |
| Agentic Memory (AgeMem) | Unifies short-/long-term memory and trains policy-level memory tool use (e.g., add, update, retrieve, summarize, filter) with progressive RL | ACL 2026 · [PDF](https://aclanthology.org/2026.acl-long.981.pdf) · [arXiv](https://arxiv.org/abs/2601.01885) · Code: not listed | External paper |

## D. Benchmarks: from recall to memory-dependent behavior

| Benchmark | What it tests | Venue · PDF · arXiv · Code |
| --- | --- | --- | --- |
| LoCoMo | Very long-term conversational memory: multi-session facts, temporal reasoning, and knowledge updates | ACL 2024 · [PDF](https://arxiv.org/pdf/2402.17753) · [arXiv](https://arxiv.org/abs/2402.17753) · [Code](https://github.com/snap-research/locomo) |
| LongMemEval | Long conversations and multi-session memory: information extraction, temporal reasoning, updates, abstention, and cross-session retrieval | ICLR 2025 · [PDF](https://arxiv.org/pdf/2410.10813) · [arXiv](https://arxiv.org/abs/2410.10813) · [Code](https://github.com/xiaowu0162/LongMemEval) |
| MemBench | Memory effectiveness, efficiency, and capacity across a more comprehensive set of memory tasks | Findings of ACL 2025 · [PDF](https://aclanthology.org/2025.findings-acl.989.pdf) · [arXiv](https://arxiv.org/abs/2506.21605) · [Code](https://github.com/import-myself/Membench) |
| MemoryAgentBench | Four memory competencies: accurate retrieval, test-time learning, long-range understanding, and selective forgetting | ICLR 2026 · [PDF](https://arxiv.org/pdf/2507.05257) · [arXiv](https://arxiv.org/abs/2507.05257) · [Code](https://github.com/HUST-AI-HYZ/MemoryAgentBench) |
| MemoryArena | Couples the agent, its memory, and an interactive environment in interdependent multi-session tasks; tests whether memory supports future actions, not only QA | ICML 2026 · [PDF](https://arxiv.org/pdf/2602.16313) · [arXiv](https://arxiv.org/abs/2602.16313) · [Code](https://github.com/ZexueHe/MemoryArena) |
| AMA-Bench | Evaluates long-context retention and long-horizon agent memory over realistic trajectories and variable task horizons | ICML 2026 · [PDF](https://arxiv.org/pdf/2602.22769) · [arXiv](https://arxiv.org/abs/2602.22769) · [Code](https://github.com/AMA-Bench/AMA-Bench) |

## E. Surveys and entry points

| Resource | Use | Venue · PDF · arXiv · Code |
| --- | --- | --- |
| A Survey on the Memory Mechanism of Large Language Model-based Agents | Taxonomy of memory forms, functions, and agent memory pipelines; useful to map a new method before comparing systems | ACM Transactions on Information Systems 2025 · [PDF](https://arxiv.org/pdf/2404.13501) · [arXiv](https://arxiv.org/abs/2404.13501) · [Survey repository](https://github.com/nuster1128/LLM_Agent_Memory_Survey) |
| Memory in the Age of AI Agents | Recent broad survey and terminology guide for memory-enabled agents | arXiv preprint 2025 · [PDF](https://arxiv.org/pdf/2512.13564) · [arXiv](https://arxiv.org/abs/2512.13564) · Code: not listed |

## How to read this area as a research program

| Stage | Core question | Compare |
| --- | --- | --- |
| Representation | What information is useful beyond the current context? | Episodes vs. facts/profiles vs. reflections vs. workflows/skills vs. linked notes |
| Write/update | Which event should alter persistent state? | Append-all vs. salience filter vs. verifier-gated write vs. learned add/update/delete/skip |
| Retrieve/use | What should be surfaced for this query or action? | Similarity vs. temporal/entity reasoning vs. graph traversal vs. learned controller |
| Maintain | How does memory stay coherent over time? | Merge, summarize, revise, decay, forget, conflict resolution, short-/long-term hierarchy |
| Prove utility | Does memory improve future behavior? | Recall score alone vs. held-out task success, action quality, retention, negative transfer, cost |

### Suggested reading path

Start with **Generative Agents → MemGPT → ExpeL** for memory stream, context hierarchy, and experiential learning. Then read **AWM → A-MEM → Mem0** to compare procedural memory, evolving linked notes, and persistent fact stores. Finally compare **MemRL → Memory-R1 → MemSkill → AgeMem** for runtime value learning, RL-trained memory operations, evolving meta-memory skills, and unified short-/long-term control; evaluate them against **LongMemEval / MemBench → MemoryAgentBench → MemoryArena / AMA-Bench**. This path separates memory *content*, memory *operations*, and evidence that memory changes downstream agent behavior.

For frozen-parameter adaptation see [Training-Free Agent Learning](../training-free-agent-learning/README.md); for policy-updating methods see [Agent Training and RL](../agent-training-rl/README.md); for skill memory and discovery see [Agent Skills](../agent-skills/README.md); and for the cross-domain evaluation map see [Benchmarks and Evaluation](../benchmarks-evaluation/README.md).

