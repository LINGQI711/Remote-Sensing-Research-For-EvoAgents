# SkillWeaver: Web Agents can Self-Improve by Discovering and Honing Skills

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/general-skills/2025/arXiv/SkillWeaver%20-%20Web%20Agents%20can%20Self-Improve%20by%20Discovering%20and%20Honing%20Skills.pdf) · [Source version](https://arxiv.org/abs/2504.07079v1)

**Venue:** arXiv preprint

**Version read:** v1

**Topic:** Discovering and refining callable web skills

## 1. What problem does it address?

Web agents spend many fragile low-level actions on recurring website operations, while manually written APIs require significant effort.

## 2. How does it solve the problem?

An exploration process proposes useful website skills, implements them as Playwright Python APIs, and practices and repairs them using execution feedback. Successful APIs form a composable library that a downstream agent can invoke.

## 3. What experiments were conducted?

- Evaluates the 812-task WebArena benchmark across five websites and real-web tasks in Online-Mind2Web.
- Compares agents without skill APIs, human-authored APIs, and transfer of learned skills to weaker models.

## 4. What are the conclusions?

Learned APIs improve task execution, with reported relative gains of 31.8% on WebArena and 39.8% on the real-web setting. These percentages are relative improvements, not percentage-point changes. Exploration and practice incur an upfront cost, and website-specific skill reuse does not by itself demonstrate transfer to arbitrary unseen websites.

**Reading pointers:** Skill discovery and honing sections; experiments from PDF page 5 onward.
