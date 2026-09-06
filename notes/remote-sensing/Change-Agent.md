# Change-Agent: Towards Interactive Comprehensive Remote Sensing Change Interpretation and Analysis

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2024/IEEE-TGRS/Change-Agent%20-%20Towards%20Interactive%20Comprehensive%20Remote%20Sensing%20Change%20Interpretation%20and%20Analysis.pdf) · [Source version](https://arxiv.org/abs/2403.19646v3)

**Venue:** IEEE Transactions on Geoscience and Remote Sensing

**Version read:** v3

**Topic:** Interactive change detection and description

## 1. What problem does it address?

Change detection masks and change captions describe complementary aspects of temporal imagery, but separate systems make comprehensive, interactive change analysis difficult.

## 2. How does it solve the problem?

A multi-level change interpretation model jointly predicts pixel-level changes and semantic descriptions. Bidirectional iterative interaction connects these outputs. An LLM agent then plans and invokes Python tools to answer requests such as locating, describing, and counting changes.

## 3. What experiments were conducted?

- Introduces LEVIR-MCI with change masks and captions and evaluates detection with mean IoU and captioning with BLEU, METEOR, ROUGE, and CIDEr.
- Studies interaction modules, positional encoding, loss balancing, and joint versus single-task learning. Interactive examples illustrate downstream analysis.

## 4. What are the conclusions?

Joint interpretation provides complementary outputs without materially sacrificing detection: Table 5 reports 86.43 mean IoU for the joint model versus 86.54 for detection alone, alongside improved caption CIDEr. Interactive examples support usability; explanations of possible causes should not be treated as experimentally validated causal inference.

**Reading pointers:** Method and experimental sections; Table 5; PDF pages 4–12.
