# Remote Sensing Research for EvoAgents

A private reading collection on remote sensing agents, reusable skills, tool exploration, and agent evolution.

**9 papers · 2025–2026 · Private repository**

The organization follows [Remote Sensing Research for Disasters](https://github.com/LINGQI711/Remote-Sensing-Research-for-Disasters): papers grouped by year, with venue labels, short descriptions, and resource links. Each paper also has a concise [reading note](notes/README.md) covering its problem, method, experiments, and conclusions.

## Archive policy

- Papers with verified conference acceptance use the conference year; other entries use the first preprint year. **arXiv preprint** means no formal acceptance was verified, not that a paper was rejected.
- Venue information was checked on **2026-09-06**, using arXiv metadata, paper front matter, and author resources. Submission statements and template styles are not acceptance evidence.
- PDFs retain the supplied versions. Notes describe those versions; newer online revisions may contain different experiments or statistics.
- Only selected public papers and their reading notes are included. Unpublished manuscripts and unrelated local material are excluded. Keep this repository **Private**.

## Papers

[2026](#2026) · [2025](#2025) · [Research themes](#research-themes) · [Reading notes](notes/README.md)

### 2026

- **HiRS-Agent: A Hierarchical Multi-Agent System for Reliable Long-Horizon Remote Sensing Task Solving** — **ACM Multimedia 2026 (accepted)** [[arXiv](https://arxiv.org/abs/2608.30672)] [[PDF](papers/2026/ACM-MM/HiRS-Agent%20-%20A%20Hierarchical%20Multi-Agent%20System%20for%20Reliable%20Long-Horizon%20Remote%20Sensing%20Task%20Solving.pdf)] [[Notes](notes/HiRS-Agent.md)] [[Author resource](https://github.com/IntelliSensing/HiRS-Agent)]
  - Organizes long-horizon remote sensing workflows into manager and specialist roles, combining step-level verification, expert tuning, and hierarchical reinforcement learning.
  - Archived version: [v1](https://arxiv.org/abs/2608.30672v1). Acceptance is confirmed by arXiv Comments and the local conference-formatted PDF.

- **XSkill: Continual Learning from Experience and Skills in Multimodal Agents** — **ICML 2026 (accepted)** [[arXiv](https://arxiv.org/abs/2603.12056)] [[PDF](papers/2026/ICML/XSkill%20-%20Continual%20Learning%20from%20Experience%20and%20Skills%20in%20Multimodal%20Agents.pdf)] [[Notes](notes/XSkill.md)] [[Author resource](https://github.com/XSkill-Agent/XSkill)]
  - Distills task-level skills and action-level experiences from visual trajectories, then retrieves and adapts both without updating model parameters.
  - Archived version: [v2](https://arxiv.org/abs/2603.12056v2). Accepted at ICML 2026 according to arXiv and the author repository; the archived PDF is preprint v2.

- **GeoForge: Non-Parametric Self-Evolving Agents for Earth-Observation Reasoning** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2608.10494)] [[PDF](papers/2026/arXiv/GeoForge%20-%20Non-Parametric%20Self-Evolving%20Agents%20for%20Earth-Observation%20Reasoning.pdf)] [[Notes](notes/GeoForge.md)]
  - Combines workflow graphs, action experiences, and skill SOPs with sensing-aware tool filtering and gated memory updates.
  - Archived version: [v1](https://arxiv.org/abs/2608.10494v1). No formal conference or journal acceptance was verified.

- **MMSkills: Towards Multimodal Skills for General Visual Agents** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2605.13527)] [[PDF](papers/2026/arXiv/MMSkills%20-%20Towards%20Multimodal%20Skills%20for%20General%20Visual%20Agents.pdf)] [[Notes](notes/MMSkills.md)] [[Author resource](https://github.com/DeepExperience/MMSkills)]
  - Binds reusable procedures to visual state cards and keyframes, consulting them in a temporary branch to guide live interaction.
  - Archived version: [v3](https://arxiv.org/abs/2605.13527v3). No formal conference or journal acceptance was verified. Notes follow archived v3.

- **OpenEarth-Agent: From Tool Calling to Tool Creation for Open-Environment Earth Observation** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2603.22148)] [[PDF](papers/2026/arXiv/OpenEarth-Agent%20-%20From%20Tool%20Calling%20to%20Tool%20Creation%20for%20Open-Environment%20Earth%20Observation.pdf)] [[Notes](notes/OpenEarth-Agent.md)] [[Author resource](https://github.com/walking-shadow/OpenEarth-Agent)]
  - Creates tools and adapts workflows to unfamiliar data, evaluating complete Earth-observation pipelines in OpenEarth-Bench.
  - Archived version: [v1](https://arxiv.org/abs/2603.22148v1). No formal conference or journal acceptance was verified.

- **RS-Claw: Progressive Active Tool Exploration via Hierarchical Skill Trees for Remote Sensing Agents** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2605.13391)] [[PDF](papers/2026/arXiv/RS-Claw%20-%20Progressive%20Active%20Tool%20Exploration%20via%20Hierarchical%20Skill%20Trees%20for%20Remote%20Sensing%20Agents.pdf)] [[Notes](notes/RS-Claw.md)]
  - Uses semantically organized skill trees and progressive disclosure to balance tool availability with context cost.
  - Archived version: [v1](https://arxiv.org/abs/2605.13391v1). The PDF states submission to IEEE, which is not evidence of journal acceptance.

- **SkillsBench: Benchmarking How Well Agent Skills Work Across Diverse Tasks** — **arXiv preprint 2026** [[arXiv](https://arxiv.org/abs/2602.12670)] [[PDF](papers/2026/arXiv/SkillsBench%20-%20Benchmarking%20How%20Well%20Agent%20Skills%20Work%20Across%20Diverse%20Tasks.pdf)] [[Notes](notes/SkillsBench.md)] [[Author resource](https://www.skillsbench.ai/)]
  - Pairs expertise-heavy tasks with skills and deterministic verifiers to measure when procedural guidance helps or hurts.
  - Archived version: [v3](https://arxiv.org/abs/2602.12670v3). No formal conference or journal acceptance was verified. Archived v3 differs from online v4; these notes do not mix their statistics.

### 2025

- **GeoEvolve: Automating Geospatial Model Discovery via Multi-Agent Large Language Models** — **arXiv preprint 2025** [[arXiv](https://arxiv.org/abs/2509.21593)] [[PDF](papers/2025/arXiv/GeoEvolve%20-%20Automating%20Geospatial%20Model%20Discovery%20via%20Multi-Agent%20Large%20Language%20Models.pdf)] [[Notes](notes/GeoEvolve.md)]
  - Combines evolutionary code search with retrieved geospatial knowledge to improve classical spatial models.
  - Archived version: [v1](https://arxiv.org/abs/2509.21593v1). No formal conference or journal acceptance was verified; a submission is not counted as acceptance.

- **RingMo-Agent: A Unified Remote Sensing Foundation Model for Multi-Platform and Multi-Modal Reasoning** — **arXiv preprint 2025** [[arXiv](https://arxiv.org/abs/2507.20776)] [[PDF](papers/2025/arXiv/RingMo-Agent%20-%20A%20Unified%20Remote%20Sensing%20Foundation%20Model%20for%20Multi-Platform%20and%20Multi-Modal%20Reasoning.pdf)] [[Notes](notes/RingMo-Agent.md)]
  - Combines RS-VL3M training data, modality-specific representations, and task-aware decoding for remote sensing perception and reasoning.
  - Archived version: [v2](https://arxiv.org/abs/2507.20776v2). Filed under first preprint year 2025. Archived v2 was revised on 2026-01-05; online v3 exists. No formal acceptance was verified.

## Research themes

| Theme | Papers | Main question |
| --- | --- | --- |
| Tool access and reliable EO execution | RS-Claw, HiRS-Agent, OpenEarth-Agent | How should agents discover, verify, replan, or create tools? |
| Experiences and non-parametric evolution | XSkill, GeoForge | How can trajectories become reusable execution knowledge? |
| Multimodal skills | MMSkills, XSkill | How should procedural knowledge connect to visual state? |
| Skill evaluation | SkillsBench | When do skills help, fail, or introduce unnecessary complexity? |
| Geospatial algorithm discovery | GeoEvolve | How can spatial knowledge guide evolutionary code search? |
| Remote sensing foundation models | RingMo-Agent | How can a model unify platforms, sensors, and reasoning tasks? |

Themes can overlap. XSkill, MMSkills, and SkillsBench are general-purpose references rather than remote-sensing-specific evaluations. RingMo-Agent focuses on a trained foundation model; GeoEvolve evolves spatial algorithms. These forms of adaptation should not be treated as identical to agent memory evolution.

## Reading notes

The [notes index](notes/README.md) links to one English Markdown file per paper. Each note answers four questions:

1. What problem does it address?
2. How does it solve the problem?
3. What experiments were conducted?
4. What are the conclusions?

Notes include selected results and short qualifications where needed, plus section/table pointers to the archived PDF. They summarize the papers; experiments have not been independently reproduced.

## Files

```text
papers/
  2026/
    ACM-MM/    # HiRS-Agent
    ICML/      # XSkill
    arXiv/     # Five preprints
  2025/
    arXiv/     # GeoEvolve and RingMo-Agent
notes/
  README.md
  <paper-name>.md
metadata.json
```

PDF filenames use full paper titles. [metadata.json](metadata.json) records titles, years, venues, summaries, source versions, reading-note paths, and SHA-256 hashes. The `.gitignore` file uses an explicit allowlist; review a paper's inclusion before adding its paths.
