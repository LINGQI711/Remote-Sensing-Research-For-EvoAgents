# Remote Sensing ChatGPT: Solving Remote Sensing Tasks with ChatGPT and Visual Models

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2024/IGARSS/Remote%20Sensing%20ChatGPT%20-%20Solving%20Remote%20Sensing%20Tasks%20with%20ChatGPT%20and%20Visual%20Models.pdf) · [Source version](https://arxiv.org/abs/2401.09083v1)

**Venue:** IGARSS 2024

**Version read:** v1

**Topic:** Language-driven orchestration of visual models

## 1. What problem does it address?

Using remote sensing models normally requires users to understand separate model interfaces and manually assemble a processing pipeline.

## 2. How does it solve the problem?

ChatGPT interprets the request, plans subtasks, calls visual models, and explains their outputs. Visual cues convert image information into text that the language model can use. The toolkit combines scene classification, land-use segmentation, detection, captioning, edge extraction, polygon simplification, and counting.

## 3. What experiments were conducted?

- Tests task planning with 138 user queries and four ChatGPT backbones. The principal planning measure checks whether the essential task is included.
- Uses models associated with AID, LoveDA, and DOTA and presents interactive examples of composed interpretation tasks.

## 4. What are the conclusions?

A language interface can connect existing visual models into useful remote sensing workflows. The reported query study primarily validates task planning, rather than establishing a common end-to-end accuracy score across all visual tasks. The system is an early orchestration baseline rather than a self-evolving skill library.

**Reading pointers:** Sections 2–3; PDF pages 2–4.
