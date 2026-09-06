# RS-Claw: Progressive Active Tool Exploration via Hierarchical Skill Trees for Remote Sensing Agents

[Library](../README.md) · [All notes](README.md) · [PDF](../papers/2026/arXiv/RS-Claw%20-%20Progressive%20Active%20Tool%20Exploration%20via%20Hierarchical%20Skill%20Trees%20for%20Remote%20Sensing%20Agents.pdf) · [Source version](https://arxiv.org/abs/2605.13391v1)

**Venue:** arXiv preprint 2026  
**Version read:** v1  
**Topic:** Hierarchical skills and active tool exploration

## 1. What problem does it address?

Listing every tool consumes context, while retrieving a small fixed subset can omit tools needed later in a long workflow. Both approaches leave tool exposure largely outside the agent’s adaptive reasoning loop.

## 2. How does it solve the problem?

Organize tool information into a three-tier skill tree: skill summaries, tool catalogs, and detailed documentation. The agent progressively explores relevant branches and loads documents before invocation. Five semantic groups cover Index, Inversion, Perception, Analysis, and Statistics. This reorganizes access to existing tools rather than learning new skills from trajectories.

## 3. What experiments were conducted?

- Earth-Bench AP and IF settings, evaluated on 234 questions after excluding 14 ChangeOS-dependent questions from the original 248.
- Compares Flat (full tool registration), RAG (a retrieved subset), and RS-Claw with GPT-5, DeepSeek-V3.1, and Qwen3-32B.
- Measures final accuracy, tool coverage/order, and input tokens per question and per turn.
- Qwen3-32B ablations randomize tool grouping or remove the skill-summary layer (2layers).

## 4. What are the conclusions?

For Qwen3-32B in AP, accuracy improves by 12.45 percentage points over Flat; input tokens per question fall from 502,119 to 70,759, about 86%. The largest token reduction is setting-specific: RAG is cheaper for some stronger backbones. The 2layers variant has better tool-matching scores but lower final accuracy, showing that better tool coverage alone does not guarantee task success.

**Reading pointers:** Section IV; Tables II–V; PDF pages 8–10. Page numbers refer to the archived PDF. Results are reported by the paper, not independently reproduced.
