# VLRS-Bench: A Vision-Language Reasoning Benchmark for Remote Sensing

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2026/arXiv/VLRS-Bench%20-%20A%20Vision-Language%20Reasoning%20Benchmark%20for%20Remote%20Sensing.pdf) · [Source version](https://arxiv.org/abs/2602.07045v2) · [Code and data](https://github.com/MiliLab/VLRS-Bench)

**Venue:** arXiv preprint 2026

**Version read:** v2

**Topic:** Cognition-, decision-, and prediction-oriented remote-sensing reasoning evaluation

## 1. What problem does it address?

Most remote-sensing multimodal benchmarks emphasize recognition, classification, or short factual answers. They provide limited coverage of causal explanation, counterfactual reasoning, spatial planning, intervention decisions, and multi-stage prediction, making it difficult to diagnose complex reasoning rather than perception alone.

## 2. How does it solve the problem?

VLRS-Bench organizes 2,000 question-answer pairs into three top-level dimensions: Cognition, Decision, and Prediction. These divide into six intermediate capabilities and 14 fine-grained tasks. Questions combine RGB imagery with remote-sensing priors such as DSM, NIR, expert masks, bounding boxes, and up to eight timestamped phases. Generation is followed by automatic filtering, cross-model checking, and review by nine remote-sensing experts.

## 3. What experiments were conducted?

- Imagery comes from 11 public datasets spanning single-time and multi-time inputs, including LoveDA, Potsdam, Vaihingen, GID15, DIOR, DOTA, FAIR1M, xView2, SECOND, miniUCD, and SpaceNet7.
- Models answer single-choice, multiple-choice, fill-in-the-blank, and true-or-false questions under a shared zero-shot protocol.
- Evaluation compares proprietary and open general MLLMs with remote-sensing models, reporting top-level, intermediate, and 14-task scores.
- Additional analysis separates static from spatiotemporal cognition, object- from scene-level prediction, and the effect of answer format.

## 4. What are the conclusions?

All evaluated models remain limited: the strongest reported general model, GPT-5.4, averages 0.439 across the fine-grained tasks. Across general MLLMs, Prediction is weakest on average at 0.278, versus 0.310 for Cognition and 0.340 for Decision. Multiple-choice and fill-in performance, 15.8% and 9.0%, trail single-choice and true-or-false performance by a wide margin. Domain-specialized models sometimes outperform much larger general models, indicating that remote-sensing priors and task alignment matter beyond parameter count. The benchmark is not pure RGB reasoning: many questions provide privileged masks, DSM, NIR, or temporal references, and it currently excludes SAR, hyperspectral imagery, and languages other than English.

**Reading pointers:** Sections 3-5; Tables 1-2 and A1-A2; Figures 1-3; PDF pages 3-12 and appendices.
