# Research Collections

[Top-level catalog](../README.md) · [Paper metadata](../metadata.json) · [All reading notes](../notes/README.md)

Collections organize the library by research question rather than by storage location, with a deliberate domain boundary: **remote-sensing and EO papers appear only in `remote-sensing-agents`**. The other mechanism collections curate general-domain agent research, including papers found online that are linked from their READMEs but are not archived locally. A general-domain paper may appear in multiple mechanism collections when its mechanism is materially relevant.

## Collection taxonomy

| ID | Collection | Inclusion boundary |
| --- | --- | --- |
| `remote-sensing-agents` | [Remote Sensing Agents](remote-sensing-agents/README.md) | EO, remote-sensing, or closely related geospatial agent systems, benchmarks, and supporting models |
| `training-free-agent-learning` | [Training-Free Agent Learning](training-free-agent-learning/README.md) | General-domain adaptation without updating the backbone model during target interactions |
| `agent-memory` | [Agent Memory](agent-memory/README.md) | General-domain storage, retrieval, compression, update, or forgetting mechanisms |
| `self-evolving-agents` | [Self-Evolving Agents](self-evolving-agents/README.md) | General-domain agents that revise memory, skills, workflows, curricula, tools, or policies |
| `agent-skills` | [Agent Skills](agent-skills/README.md) | General-purpose skill representation, discovery, validation, routing, composition, and evaluation |
| `agent-training-rl` | [Agent Training and RL](agent-training-rl/README.md) | General-domain SFT, preference optimization, RL, and other parameter-updating agent training |
| `multi-agent-orchestration` | [Multi-Agent and Orchestration](multi-agent-orchestration/README.md) | General-domain roles or agents coordinated through hierarchy, delegation, debate, or specialist routing |
| `benchmarks-evaluation` | [Benchmarks and Evaluation](benchmarks-evaluation/README.md) | General-domain datasets, environments, metrics, protocols, and diagnostic studies for agent behavior |

## Maintenance rules

1. Store each PDF once under `papers/` and each detailed note once under `notes/`.
2. Keep EO/remote-sensing papers only in `remote-sensing-agents`; mechanism collections are for general-domain agent work.
3. Add a general-domain paper to every mechanism collection whose mechanism is materially evaluated, not merely mentioned. External references can be listed in collection READMEs without duplicating PDFs or notes.
4. Distinguish parameter-free adaptation from trained agents; a method can combine both and should state which component is trained.
5. Treat benchmark scores as protocol-specific. Record backbone, task split, tool inventory, retry policy, and metric whenever comparisons depend on them.
6. Update [catalog.json](catalog.json) when adding or removing locally archived paper membership.

## Suggested research path

Start with [Training-Free Agent Learning](training-free-agent-learning/README.md), then follow the mechanism chain:

```text
experience -> memory -> skill extraction -> skill validation/routing
           -> workflow or policy update -> self-evolution -> evaluation
```

Use [Remote Sensing Agents](remote-sensing-agents/README.md) as the EO application collection. The mechanism collections and [Benchmarks and Evaluation](benchmarks-evaluation/README.md) focus on general-domain evidence.
