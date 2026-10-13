# TriSV-CD: Selective verification with a do-no-harm arbitration gate for reliable remote sensing change detection

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2027/ESWA/TriSV-CD%20-%20Selective%20verification%20with%20a%20do-no-harm%20arbitration%20gate%20for%20reliable%20remote%20sensing%20change%20detection.pdf) · [Publication](https://doi.org/10.1016/j.eswa.2026.134443)

**Venue:** Expert Systems with Applications 334 (2027), article 134443

**Version read:** published version

**Topic:** Reliable change-detection verification, rollback, and VLM decision auditing

## 1. What problem does it address?

Post-hoc change-detection correction can improve average F1 while harming individual samples. VLMs can describe disputed regions, but a fluent accept-or-rollback judgment may be prompt-sensitive. Average benchmark scores do not expose the harmful-edit rate, the confidence structure of failures, or the gap to an oracle that chooses the better of the baseline and correction proposal for each sample.

## 2. How does it solve the problem?

The paper first audits Qwen2.5-VL under multiple decision and description prompts and separates semantic diagnosis from deployment-time arbitration. V4-Safe then compares a baseline probability map with a test-time-augmentation correction proposal. It computes the mean baseline probability on the proposal's edited support and rolls back edits in high-confidence regions. The gate is training-free and does not call a VLM at deployment.

## 3. What experiments were conducted?

- Five change-detection backbones are evaluated on SYSU-CD, LEVIR-CD, and NJDS, producing a complete 5-by-3 backbone-dataset matrix.
- Metrics include mean per-sample F1 change, harmful-edit rate, correction precision, oracle gap, Wilcoxon tests with Holm correction, and paired bootstrap intervals.
- VLM prompts, VLM-informed class-specific thresholds, generic rejection rules, threshold sensitivity, probability-scale transfer, and zero-shot cross-domain checkpoints are audited separately.

## 4. What are the conclusions?

Direct VLM decisions vary sharply with prompt wording; on 182 coordinates shared by three decision formulations, pairwise three-way agreement is 0%. Adding VLM semantic classes to a threshold gate does not outperform the probability-only rule, and 92% of 1,000 shuffled-label controls match or exceed the original class-informed F1 change. V4-Safe produces positive mean F1 changes in 13 of 15 matrix cells, an exact no-op in one degenerate cell, and a statistically indistinguishable negative change in one cell. Harmful-edit rate falls from 41.90% to 7.68% for PDEFM-SYSU and from 10.87% to 4.88% for BIT-NJDS. These results support transparent rollback controls and richer reliability metrics, but not a universal guarantee: the fixed threshold is sensitive to backbone and domain probability scales, and the full test-time-augmentation pipeline is substantially slower than baseline inference.

**Reading pointers:** Sections 3-6; Tables 1-10, 14, and 22; Figures 1 and 3-6; PDF pages 3-17.
