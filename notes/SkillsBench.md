# SkillsBench: Benchmarking How Well Agent Skills Work Across Diverse Tasks

[Library](../README.md) · [All notes](README.md) · [PDF](../papers/2026/arXiv/SkillsBench%20-%20Benchmarking%20How%20Well%20Agent%20Skills%20Work%20Across%20Diverse%20Tasks.pdf) · [Source version](https://arxiv.org/abs/2602.12670v3)

**Venue:** arXiv preprint 2026  
**Version read:** v3  
**Topic:** Benchmarking the effectiveness of agent skills

## 1. What problem does it address?

Skill libraries are widely used, but their practical value is difficult to compare without matched tasks, executable evaluation, and controls for model and harness differences.

## 2. How does it solve the problem?

Build containerized tasks with instructions, reusable skill resources, oracle solutions, and deterministic verifiers. Apply automated and human quality checks, including leakage controls. Compare the same model–harness configuration without skills, with curated skills, and with skills generated before attempting a task.

## 3. What experiments were conducted?

- The evaluation uses 84 tasks across 11 domains, seven model–harness configurations spanning Claude Code, Gemini CLI, and Codex CLI, and 7,308 valid trajectories.
- Pass rate averages binary outcomes over five trials per task, then over tasks; normalized gain complements absolute percentage-point improvement.
- Self-generated skills are evaluated for five configurations; Gemini CLI is excluded from that condition.
- Analyses cover domains, individual tasks, skill count, documentation complexity, model scale, and cost.

## 4. What are the conclusions?

Section 4 reports an average curated-skill gain of about 16.2 percentage points; 16 of 84 tasks nevertheless regress. Self-generation before solving provides little or negative average benefit. Tasks with focused skill bundles show stronger gains than those with larger bundles, but this grouped analysis does not establish a universal optimal skill count. Version caveat: the abstract says 86 tasks, while evaluation uses 84; Figure 2 reports +12.66 pp rather than the main text’s +16.2 pp. Use the specific table/protocol when citing numbers. This is not a test of trajectory-based skill evolution.

**Reading pointers:** Sections 2.5–4.2; Tables 3–6 and Figure 2; PDF pages 4–7.
