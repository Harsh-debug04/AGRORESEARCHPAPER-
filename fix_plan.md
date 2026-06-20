# Fix Plan

## Critical Issues From README / Review Docs
| Issue ID | Source file | Problem summary | Affected section(s) | Evidence source(s) | Action required | Risk if not fixed |
|---|---|---|---|---|---|---|
| 1 | Review/README | Overclaimed real-world agronomic validation (15-20% N reduction) | Abstract, Intro, 7.3, 8.2 | README, Review | Soften claim; state explicitly it's a simulation, not real-world data. Remove claims of farmer impact. | Rejection due to unverified claims. |
| 2 | README | Opaque hallucination evaluation (<2% on 500 queries) | 7.2 | README | Acknowledge limited scope of adversarial queries (banned substances) and lack of formal rubric. | Rejection due to irreproducibility. |
| 3 | Review | Authorship inconsistency | Title page, CRediT | Review, TASK.md | Standardize author names to Aarav Asthana and Suyash Sinha. | Rejection due to integrity concerns. |
| 4 | README | Weak LoRA fine-tuning dataset wording ('generated') | 5.5 | README | Rewrite Section 5.5 to emphasize manual curation; use README text. | Rejection due to synthetic data concerns. |
| 5 | README | Missing Section 5.5 dataset statistics table | 5.5 | README | Add Table with estimated/approximate stats for clarity. | Reviewer skepticism. |
| 6 | README | Missing quality-control statement for dataset curation | 5.5 | README | Add text about cross-checking and validation by annotators. | Lack of rigor. |
| 7 | Review | Retrieval quality not evaluated (only latency) | 7.1 | Review | Add limitation stating retrieval relevance was not measured. | Rejection due to incomplete evaluation. |
| 8 | Review | No proper RAG vs LoRA vs combined ablation | 7.2 | Review, Ablation Guide | Clarify that LoRA-only was not tested; discuss RAG+LoRA as a combined pipeline. | Weak contribution claim. |
| 9 | Review | Carbon-footprint module overclaimed | 5.4 | Review | Reframe as a basic IPCC Tier 1 implementation for proof-of-concept. | Rejection due to triviality masquerading as novelty. |
| 10 | Review | Multilingual capability overclaimed | 1, 8 | Review | Reframe 22 languages as an embedding capability, not evaluated performance. | Rejection due to unsupported claims. |
| 11 | Review | Citation / benchmark / timeline inconsistencies | Related Work | Review | Remove 2026 citations; clarify that GPT-4o-mini is an estimate or remove it. | Rejection due to fabricated timelines. |

## Rewrite Strategy
### Sections to fully rewrite
- Abstract: to scope down claims, specify simulation.
- Introduction: to remove unverified deployment impact claims.
- Section 5.5 (Fine-tuning Dataset): to replace 'generated' with manual curation details, add stats table, and quality control.

### Sections to heavily revise
- Section 7.2 (Hallucination): to be honest about the limited scope of the 500 queries.
- Section 7.3 (Agronomic Impact): to clearly label it as a simulation.
- Section 8 (Discussion): to include limitations on retrieval evaluation, multilingual testing, and real-world impact.
- CRediT Authorship: to fix names.

### Sections to keep with minor edits
- System Architecture (except Carbon Footprint framing).
- LoRA methodology (ensure no overclaiming).

### Claims to soften or remove
- 15-20% nitrogen reduction (soften to simulation).
- 22-language support (soften to infrastructure capability).
- <2% hallucination (soften to 'on a limited set of banned-substance queries').
- Hyper-localized (remove/soften as it was only 3 districts).

### New tables / figures / appendices to add
- Dataset Statistics Table in Section 5.5.
