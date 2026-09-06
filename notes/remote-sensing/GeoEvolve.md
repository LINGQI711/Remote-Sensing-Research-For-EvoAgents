# GeoEvolve: Automating Geospatial Model Discovery via Multi-Agent Large Language Models

[Library](../../README.md) · [Part index](README.md) · [All notes](../README.md) · [PDF](../../papers/remote-sensing/2025/arXiv/GeoEvolve%20-%20Automating%20Geospatial%20Model%20Discovery%20via%20Multi-Agent%20Large%20Language%20Models.pdf) · [Source version](https://arxiv.org/abs/2509.21593v1)

**Venue:** arXiv preprint 2025

**Version read:** v1

**Topic:** Automated geospatial algorithm discovery

## 1. What problem does it address?

Generic code-evolution systems can search algorithms without understanding spatial dependence or uncertainty. Unstructured domain prompts may not provide knowledge relevant to the model being optimized.

## 2. How does it solve the problem?

Use an inner code-evolution loop to generate and mutate candidates and an outer multi-agent controller to assess elites and query GeoKnowRAG. Retrieved spatial theory guides further search. An executable evaluator scores candidate models; the evolved object is algorithm code, not an agent’s reusable tool-use memory.

## 3. What experiments were conducted?

- Ordinary kriging for Australian copper, lead, and zinc observations; evaluates RMSE, MAE, and R-squared.
- Geospatial conformal prediction (GeoCP) for Seattle/King County housing-price uncertainty, with XGBoost as the underlying predictor; evaluates interval score, which balances width and coverage penalties.
- Compares original algorithms, OpenEvolve, OpenEvolve with geospatial prompts, GeoEvolve without GeoKnowRAG, and the full system. Inspects the resulting algorithm modifications.

## 4. What are the conclusions?

Relative to original kriging, reported RMSE reductions are 15.4%, 21.2%, and 13.0% for Cu, Pb, and Zn. GeoCP interval score falls from 55.37 to 46.12, a 16.7% reduction. Retrieval-guided evolution improves the tested objectives. Table 1 does not show uniform gains on every metric: Zn R-squared is lower for the full system. The evidence in this version covers two algorithm families, not general EO workflow automation.

**Reading pointers:** Sections 4–5; Tables 1–2; PDF pages 6–10.
