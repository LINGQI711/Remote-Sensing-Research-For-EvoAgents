# Agent Mechanism Research Library

A structured paper library for studying **how agents learn, remember, evolve, acquire skills, coordinate, and are evaluated**, with remote sensing as a major application domain.

The repository currently contains **38 reviewed papers**: **26 remote-sensing papers** and **12 general agent-mechanism papers**. Every archived paper has a local PDF, structured metadata, and an English reading note.

## Research collections

| Collection | Core question | Entry point |
| --- | --- | --- |
| Remote Sensing Agents | How are agents designed and evaluated for Earth observation and geospatial workflows? | [Open collection](collections/remote-sensing-agents/README.md) |
| Training-Free Agent Learning | How can a frozen backbone improve through experience, prompts, workflows, tools, or external state? | [Open collection](collections/training-free-agent-learning/README.md) |
| Agent Memory | What should an agent store, retrieve, update, compress, and forget? | [Open collection](collections/agent-memory/README.md) |
| Self-Evolving Agents | How can agents revise their own memory, skills, workflows, or tool-use policies over time? | [Open collection](collections/self-evolving-agents/README.md) |
| Agent Skills | How are reusable skills represented, discovered, validated, routed, and composed? | [Open collection](collections/agent-skills/README.md) |
| Agent Training and RL | Which capabilities require parameter updates, supervised trajectories, or reinforcement learning? | [Open collection](collections/agent-training-rl/README.md) |
| Multi-Agent and Orchestration | When does role specialization, hierarchy, debate, or manager-worker coordination help? | [Open collection](collections/multi-agent-orchestration/README.md) |
| Benchmarks and Evaluation | How should agent outcomes, trajectories, tools, parameters, cost, and transfer be measured? | [Open collection](collections/benchmarks-evaluation/README.md) |

## Repository map

```text
.
├── README.md                         # This top-level catalog
├── collections/                      # Cross-cutting research-topic indexes
│   ├── README.md                     # Taxonomy and maintenance rules
│   ├── catalog.json                  # Machine-readable many-to-many membership
│   └── <research-topic>/README.md    # One curated topic collection
├── papers/                           # Canonical local PDF archive
│   ├── remote-sensing/
│   └── general-skills/
├── notes/                            # Canonical paper-by-paper reading notes
│   ├── remote-sensing/
│   └── general-skills/
└── metadata.json                     # Canonical bibliographic and file metadata
```

## Canonical indexes

- [All research collections](collections/README.md)
- [All paper reading notes](notes/README.md)
- [Remote-sensing notes](notes/remote-sensing/README.md)
- [General mechanism and skill notes](notes/general-skills/README.md)
- [Machine-readable paper metadata](metadata.json)
- [Machine-readable collection membership](collections/catalog.json)

## Organization principle

PDFs and individual notes have one canonical location. Collection READMEs are thematic views over the same assets, so a paper may appear in several collections without duplicating its PDF or note. This separates **application domains** from **agent mechanisms** and makes the library usable for both remote-sensing research and general agent research.
