# OpenEarthAgent: A Unified Framework for Tool-Augmented Geospatial Agents

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/arXiv/OpenEarthAgent%20-%20A%20Unified%20Framework%20for%20Tool-Augmented%20Geospatial%20Agents.pdf) · [Source version](https://arxiv.org/abs/2602.17665v4)

**Venue:** arXiv preprint

**Version read:** v4

**Topic:** Training compact geospatial tool-using agents

## 1. What problem does it address?

Small language models often fail to select geospatial tools, fill their arguments, or preserve the required execution order.

## 2. How does it solve the problem?

The framework standardizes tool schemas and builds validated trajectories across optical, SAR, and GIS tasks. It trains Qwen3-4B on 14,538 examples using supervised, response-only learning, with tool outputs retained as context. Evaluation contains 1,169 examples. This is distinct from OpenEarth-Agent, the separately indexed tool-creation paper.

## 3. What experiments were conducted?

- Separates step-by-step evaluation using supplied context from end-to-end execution with live tools.
- Compares frontier and open models using tool arguments, tool-category F1, sequence matching, and final answers; also tests transfer to Earth-Agent and ThinkGeo.

## 4. What are the conclusions?

Targeted trajectory training substantially improves a compact model: end-to-end answer accuracy rises from 13.72 to 45.26, and exact tool-sequence accuracy from 14.71 to 67.24 against its base model. It does not lead every metric, including image-generation accuracy. Stepwise scores should not be mistaken for autonomous end-to-end success.

**Reading pointers:** Sections 3–4; Tables 3–5; PDF pages 7–14.
