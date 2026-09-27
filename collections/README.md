# Research Collections

[Top-level catalog](../README.md) · [Paper metadata](../metadata.json) · [All reading notes](../notes/README.md)

Collections organize the library by research question rather than by storage location. They are intentionally **many-to-many**: a paper can study memory, self-evolution, and skills at the same time.

## Collection taxonomy

| ID | Collection | Inclusion boundary |
| --- | --- | --- |
| `remote-sensing-agents` | [Remote Sensing Agents](remote-sensing-agents/README.md) | EO, remote-sensing, or closely related geospatial agent systems, benchmarks, and supporting models |
| `training-free-agent-learning` | [Training-Free Agent Learning](training-free-agent-learning/README.md) | Adaptation without updating the backbone model during the target task sequence |
| `agent-memory` | [Agent Memory](agent-memory/README.md) | Explicit storage, retrieval, compression, update, or forgetting mechanisms that affect later behavior |
| `self-evolving-agents` | [Self-Evolving Agents](self-evolving-agents/README.md) | Agents that change external knowledge, skills, workflows, tools, or policies using interaction evidence |
| `agent-skills` | [Agent Skills](agent-skills/README.md) | Reusable procedural units and their discovery, representation, validation, routing, composition, or evaluation |
| `agent-training-rl` | [Agent Training and RL](agent-training-rl/README.md) | SFT, preference optimization, RL, hierarchical objectives, or other parameter-updating agent training |
| `multi-agent-orchestration` | [Multi-Agent and Orchestration](multi-agent-orchestration/README.md) | Multiple roles or agents coordinated through hierarchy, delegation, debate, or specialist routing |
| `benchmarks-evaluation` | [Benchmarks and Evaluation](benchmarks-evaluation/README.md) | Datasets, environments, metrics, protocols, and diagnostic studies for agent behavior |

## Maintenance rules

1. Store each PDF once under `papers/` and each detailed note once under `notes/`.
2. Add a paper to every collection whose mechanism is materially evaluated, not merely mentioned.
3. Distinguish parameter-free adaptation from trained agents; a method can combine both and should state which component is trained.
4. Treat benchmark scores as protocol-specific. Record backbone, task split, tool inventory, retry policy, and metric whenever comparisons depend on them.
5. Update [catalog.json](catalog.json) when adding or removing collection membership.

## Suggested research path

Start with [Training-Free Agent Learning](training-free-agent-learning/README.md), then follow the mechanism chain:

```text
experience -> memory -> skill extraction -> skill validation/routing
           -> workflow or policy update -> self-evolution -> evaluation
```

Use [Remote Sensing Agents](remote-sensing-agents/README.md) as the application testbed and [Benchmarks and Evaluation](benchmarks-evaluation/README.md) to compare evidence.
