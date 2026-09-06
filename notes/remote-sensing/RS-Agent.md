# RS-Agent: Automating Remote Sensing Tasks through Intelligent Agent

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/SCIS/RS-Agent%20-%20Automating%20Remote%20Sensing%20Tasks%20through%20Intelligent%20Agent.pdf) · [Source version](https://arxiv.org/abs/2406.07089v4)

**Venue:** Science China Information Sciences

**Version read:** v4

**Topic:** Domain knowledge and remote sensing tool orchestration

## 1. What problem does it address?

General multimodal models struggle to translate remote sensing requests into professional workflows that require specialized models, multiple data sources, and domain knowledge.

## 2. How does it solve the problem?

A central controller coordinates a dynamic toolkit, a solution space of expert workflows, and a knowledge space. Task-Aware Retrieval first identifies the task and then retrieves suitable solutions. DualRAG combines complementary retrieval paths to supply domain evidence. The controller uses these resources to plan and execute optical and SAR workflows.

## 3. What experiments were conducted?

- Evaluates 18 remote sensing tasks, including scene classification, visual question answering, object counting, and multi-tool planning.
- Compares proprietary and open language models and ablates task inference, solution retrieval, and their combination.
- Separately compares DualRAG with LightRAG on RSaircraft and UltraDomain Mix, evaluating knowledge-response quality.

## 4. What are the conclusions?

Expert workflow retrieval substantially improves planning: the combined retrieval configuration reaches 90.62% multi-tool planning accuracy versus 9.42% for the baseline in Table 6. Knowledge-retrieval gains vary by dataset and metric. This is evidence for domain-guided orchestration; it does not establish continual skill learning from agent experience.

**Reading pointers:** Section 4; Tables 6 and 8; PDF pages 8–14.
