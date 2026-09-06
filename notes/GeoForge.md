# GeoForge: Non-Parametric Self-Evolving Agents for Earth-Observation Reasoning

[Library](../README.md) · [All notes](README.md) · [PDF](../papers/2026/arXiv/GeoForge%20-%20Non-Parametric%20Self-Evolving%20Agents%20for%20Earth-Observation%20Reasoning.pdf) · [Source version](https://arxiv.org/abs/2608.10494v1)

**Venue:** arXiv preprint 2026  
**Version read:** v1  
**Topic:** Non-parametric evolution for Earth observation

## 1. What problem does it address?

Earth-observation workflows must respect sensor modalities, products, parameters, and intermediate dependencies. Generic tool search and unstructured trajectory memories fail to preserve these constraints across tasks.

## 2. How does it solve the problem?

Filter the tool space using the sensing context, then retrieve a task-conditioned prior from three memories: Workflow Graph Memory, Action-Level Experiences, and adapted Skill SOPs. Execute against current observations, then use safety-gated distillation to convert grounded trajectories into reusable knowledge. The backbone remains frozen; evolution occurs in external execution memory.

## 3. What experiments were conducted?

- Earth-Bench comparisons across five LLM backbones against Earth-Agent and other EO agents, using final accuracy and tool-trajectory metrics.
- ThinkGeo and GeoPlan-Bench extend evaluation to instruction/tool/argument correctness and higher-level workflow planning.
- Component ablations remove graph, skill, and experience memory. Additional analyses compare spectrum, derived-product, and RGB tasks, including general-purpose agent baselines.

## 4. What are the conclusions?

The paper reports the best Earth-Bench accuracy on four of five tested backbones; GPT-5 reaches 74.33% versus 63.16% for Earth-Agent. Memory ablations support complementary roles for task knowledge and workflow structure. Gains are not uniform across every metric or modality: Table 4 reports lower RGB accuracy than Earth-Agent despite a higher overall average. The experiments support structured memory reuse within these benchmarks, not unrestricted long-term autonomy.

**Reading pointers:** Experiments; Tables 1–4; PDF pages 5–6. Page numbers refer to the archived PDF. Results are reported by the paper, not independently reproduced.
