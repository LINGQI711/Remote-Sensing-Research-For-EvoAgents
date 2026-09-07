# Evaluating Tool-Augmented Agents in Remote Sensing Platforms

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2024/ICLR-Workshops/Evaluating%20Tool-Augmented%20Agents%20in%20Remote%20Sensing%20Platforms.pdf) · [Source version](https://arxiv.org/abs/2405.00709v1)

**Venue:** ICLR 2024 Workshops · ML4RS

**Version read:** v1

**Topic:** State-aware remote sensing platform agent evaluation

## 1. What problem does it address?

Static image-question pairs omit the live platform state implied by requests such as detecting objects in the currently selected map area. Agents must track that state and execute complete tool sequences.

## 2. How does it solve the problem?

GeoLLM-QA represents a task using the user question, tool-call sequence, response, and final platform state. It constructs 1,000 tasks with 117 tools and uses oracle detections from annotated data to isolate agent errors from detector errors.

## 3. What experiments were conducted?

- Compares GPT-3.5 Turbo and GPT-4 Turbo with CoT, ReAct, and Chameleon in zero-shot and few-shot settings.
- Measures task success, tool-call correctness, textual response quality, detection recall, and token cost.
- Table 1 reports GPT-4's best task success as 34.99% with zero-shot CoT, while its highest tool correctness is 94.98% with few-shot ReAct.

## 4. What are the conclusions?

Correct individual calls and plausible responses are insufficient for successful end-to-end execution. Omitted calls are a major failure mode. Because detections are provided by an oracle, the results do not measure robustness to real detector noise. This is distinct from GeoLLM-Engine and GeoLLM-Squad.

**Reading pointers:** Section 2 for the platform, oracle detectors, and task construction; Section 3, Table 1, and Figure 3 for results and errors; Section 4 for future work.
