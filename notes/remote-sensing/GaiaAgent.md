# Towards comprehensive multi-task land cover change detection leveraging vision-language model and LLM-driven agents

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/ISPRS-JPRS/Towards%20comprehensive%20multi-task%20land%20cover%20change%20detection%20leveraging%20vision-language%20model%20and%20LLM-driven%20agents.pdf) · [Source version](https://doi.org/10.1016/j.isprsjprs.2026.05.025)

**Venue:** ISPRS Journal of Photogrammetry and Remote Sensing

**Version read:** Published version, volume 238, pages 756-774

**Topic:** Multi-agent 2D/3D land-cover change analysis

## 1. What problem does it address?

Land-cover change studies often separate 2D semantic changes, 3D structural changes, and downstream impact analysis. The paper targets an interactive workflow that connects these stages.

## 2. How does it solve the problem?

UrbanChange combines optical imagery, height information, semantic changes, and change captions. A vision-language perception model learns with textual guidance and uses its visual branch at inference. GaiaAgent coordinates five roles for planning, data preparation, detection, analysis, and user-guided revision. The planner includes an understanding-correction mechanism.

## 3. What experiments were conducted?

- Evaluates 2D and 3D change detection on UrbanChange, including comparisons with existing detectors and ablations of textual guidance.
- Examines interactive downstream analysis and instruction-to-plan consistency.
- Table 10 tests ten semantically equivalent instructions: understanding-correction increases correct executions from 7/10 to 9/10.

## 4. What are the conclusions?

The work connects multi-dimensional change perception to interactive quantitative analysis. Detection-model improvements and agent-workflow reliability are separate results: the small instruction test does not establish broad agent robustness. The authors identify restricted task coverage and lack of support for external analytical tools as limitations; dynamic tool discovery remains future work.

**Reading pointers:** Sections 3-4 for UrbanChange, perception, and agent roles; Section 5 for detection experiments; Section 6.2 and Table 10 for planner correction; Section 6.4 for scope limitations.
