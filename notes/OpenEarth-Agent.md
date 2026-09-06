# OpenEarth-Agent: From Tool Calling to Tool Creation for Open-Environment Earth Observation

[Library](../README.md) · [All notes](README.md) · [PDF](../papers/2026/arXiv/OpenEarth-Agent%20-%20From%20Tool%20Calling%20to%20Tool%20Creation%20for%20Open-Environment%20Earth%20Observation.pdf) · [Source version](https://arxiv.org/abs/2603.22148v1)

**Venue:** arXiv preprint 2026  
**Version read:** v1  
**Topic:** Tool creation for open-environment Earth observation

## 1. What problem does it address?

An EO agent limited to a fixed tool registry cannot readily handle new sensors, data conventions, or scientific tasks. Correctness must also survive the transition from data preparation to analysis.

## 2. How does it solve the problem?

Coordinate data summarization, planning/workflow construction, code-based tool creation, and result checking. Incorporate external tools and domain knowledge as needed, and use execution feedback to debug generated procedures. The core change is to synthesize task-specific functionality rather than depend exclusively on predefined APIs.

## 3. What experiments were conducted?

- Introduces OpenEarth-Bench: 596 cases across seven domains, with data preparation, feature extraction, and geospatial analysis evaluated both stage-wise and end-to-end.
- Tests six backbones: GPT-5, Gemini-2.5-Flash, Kimi K2, DeepSeek-V3.1, Qwen3-Max, and Seed-1.6. Reports accuracy, debugging rounds, and runtime.
- On Earth-Bench, compares Earth-Agent with variants given only six essential pretrained model tools or the complete toolset; external knowledge/tool integration is disabled for this comparison.
- Ablates specialized agents and open knowledge/tool integration; examines failures in sensor assumptions, masking, and numerical processing.

## 4. What are the conclusions?

With GPT-5 on Earth-Bench, accuracy is 59.92% with six tools and 67.61% with full tools, versus Earth-Agent at 63.16%. Thus the minimal-tool setting is competitive but does not exceed that baseline. Cascading errors remain substantial: GPT-5 geospatial analysis falls from 76.66% stage-wise to 58.72% end-to-end. Tool creation increases flexibility, but reliable complete pipelines remain difficult.

**Reading pointers:** Sections 4–5; Tables 2–4 and Figure 4; PDF pages 7–12.
