# REMSA: Foundation Model Selection for Remote Sensing via a Constraint-Aware Agent

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2025/arXiv/REMSA%20-%20Foundation%20Model%20Selection%20for%20Remote%20Sensing%20via%20a%20Constraint-Aware%20Agent.pdf) · [Source version](https://arxiv.org/abs/2511.17442v3) · [Code](https://github.com/be-chen/REMSA)

**Venue:** arXiv preprint

**Version read:** v3

**Topic:** Constraint-aware remote sensing foundation-model selection

## 1. What problem does it address?

Selecting a remote sensing foundation model requires reconciling scattered documentation with task, modality, data, and compute constraints. Similarity retrieval alone does not ensure a suitable recommendation.

## 2. How does it solve the problem?

REMSA grounds natural-language requests in RS-FMD, a structured database covering over 160 models. A task-aware orchestrator combines retrieval, hard-constraint filtering, clarification, in-context ranking, and explanations linked to model evidence.

## 3. What experiments were conducted?

- Uses 100 expert-verified queries and expert suitability ratings, comparing REMSA with a naive agent, database retrieval, and unstructured RAG.
- Evaluates GPT-4.1, DeepSeek3.2, and LLaMA-3.3-70B backbones and sensitivity to evaluation criteria.
- With GPT-4.1, Table 2 reports an average Top-1 score of 75.76 and a 40.00% high-quality hit rate; database retrieval obtains 67.37 and 17.33%, respectively.

## 4. What are the conclusions?

Structured grounding plus multi-stage decisions improves expert-scored recommendation quality, at greater latency than retrieval alone. These scores measure perceived model suitability, not accuracy after adapting the selected model to the user's data. The benchmark's query coverage and dependence on metadata remain important boundaries.

**Reading pointers:** Sections 3-4 for RS-FMD and orchestration; Sections 5-6 and Table 2 for the expert evaluation; Section 7 for limitations. Filed under the initial preprint year 2025; the archived PDF is v3 from June 2026.
