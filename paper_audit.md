# Paper Audit

## Repository Map
| File | Type | Why it matters to the paper | Priority |
|---|---|---|---|
| README.md | Markdown | Critical reviewer instructions on major flaws | High |
| RESEARCH PAPER PDF.pdf | PDF | The current paper to be rewritten | High |
| AgroTrack_Ablation_Study_Guide.docx | DOCX | Instructions on how the ablation section should look/be done | High |
| AgroTrack_Q1_Review_Report.docx | DOCX | Detailed peer review identifying major gaps to fix | High |
| Agriculture Organisation.xlsx | Excel | Contains data potentially relevant for dataset statistics | Medium |
| TASK.md | Markdown | Non-negotiable output rules for final generation | High |

## Section-by-Section Defect Audit
| Section | Current claim/content | Problem | Severity | Evidence available? | Planned fix |
|---|---|---|---|---|---|
| Title | AgroTrack: A Retrieval-Augmented Generation Framework for Dynamic, Hyper-Localized Crop Calendar Intelligence in Smallholder Agriculture | Claims hyper-localized intelligence but only piloted in 3 districts (1 agro-climatic zone) | Medium | No evidence for hyper-localization | Adjust title to reflect the actual scope. |
| Abstract | Claims 15-20% nitrogen reduction | It is a simulation, not real-world data | High | Simulation only | Rewrite to explicitly state it's a simulation. |
| Introduction | Cites 15-20% reduction and 1,200 farmer deployment | Conflates deployment with agronomic impact | High | No agronomic impact data | Clarify that deployment is for system latency/infrastructure testing, not agronomic outcomes. |
| Related Work | Cites papers from 2026 (Mukti et al., Piazolo et al.) | Impossible timeline, reviewer flagged | High | No | Remove/replace with actual relevant 2024/2025 papers on LLMs in agriculture. |
| Dataset (5.5) | '12,000 instruction-output pairs generated from ICAR' | Implies synthetic data, reviewer flagged | Critical | Yes (README) | Rewrite using manual curation text from README; add statistics table and quality control statement. |
| Evaluation (Hallucination) | <2% hallucination rate on 500 adversarial queries | Opaque methodology, no rubric or evaluator details | High | No detailed rubric | Soften claim; state limitation of evaluating only banned pesticides and need for broader agronomic evaluation. |
| Evaluation (Retrieval) | Claims good retrieval based on <50ms latency | Latency is not quality (no MRR, NDCG) | High | No retrieval metrics | State that retrieval latency was measured but retrieval relevance/quality is a limitation/future work. |
| Evaluation (Ablation) | Shows Base vs RAG vs RAG+LoRA | Missing LoRA-only condition, cannot prove LoRA independent contribution | High | No LoRA-only data in paper | Adjust ablation claims to reflect available data or state missing LoRA-only as limitation. |
| Multilingual | Claims support for 22 languages | Never evaluated, just asserted | High | No multilingual evaluation | Reframe as infrastructure capability (encoder support) rather than validated performance. |
| Carbon Footprint | Equation 3 presented as novel module | Trivial IPCC Tier 1 formula, overclaimed | Medium | Yes, it's just a formula | Reframe as a proof-of-concept sustainability feature, not a major novel contribution. |
| Authorship | Byline: Aarav/Suyash; CRediT: Aryan/Priya/Devraj | Inconsistent authors | Critical | TASK.md mandates fixing | Standardize authors to Aarav Asthana and Suyash Sinha throughout. |
