# Final Change Log

## Major paper changes
- Title scoping adjusted to reflect evaluation scope.
- Abstract and Introduction: Removed unverified claims about real-world agronomic impacts; clearly stated that the nitrogen reduction results are from a simulation, and the 1,200-farmer pilot was a latency/load test.
- Reframed 'Carbon-Footprint Modelling' as a basic/proof-of-concept IPCC Tier 1 feature.

## README / review issues resolved
- Replaced 'generated' text in dataset description with accurate manual curation text.
- Resolved authorship inconsistency by standardizing to Aarav Asthana and Suyash Sinha.
- Removed 2026 citations from Related Work to correct impossible timeline.
- Acknowledged lack of retrieval evaluation (MRR/NDCG).

## Claims softened or removed
- '15-20% nitrogen reduction' softened to a simulation outcome.
- '<2% hallucination rate' softened to clarify it only applies to a specific set of adversarial queries on banned substances, with no formal rubric yet.
- '22 Indian languages' reframed as an infrastructural capability (via the encoder) rather than evaluated performance.
- 'Hyper-localized' claim softened.

## New additions
- Dataset statistics table added to Section 5.5.
- Quality-control paragraph added to Section 5.5.
- Ablation clarification (combined pipeline vs independent LoRA).

## Remaining limitations
- Lack of real-world randomized controlled field trial.
- Absence of formal hallucination rubric and broader agronomic evaluation.
- Lack of retrieval relevance evaluation.
- Lack of multilingual evaluation.

## Output files created
- `research_paper_final.tex`
- `RESEARCH PAPER FINAL PDF.pdf`
- `paper_audit.md`
- `fix_plan.md`
- `evidence_claim_matrix.md`
- `final_change_log.md`

## Comparative LLM study additions
- candidate models compared: Mistral Large 2 (123B), Llama-3-70B, Qwen-2-72B
- metrics added: Outlined a comparative evaluation framework involving Agronomic Factuality, Groundedness, Retrieval Utilization, and Latency/Efficiency.
- tables added: No new data tables for LLM comparison due to lack of evidence in the repo.
- graphs added: N/A
- best-performing model and rationale: Mistral Large 2 was retained as the default due to its pre-existing context window and multilingual pretraining within the repo; however, a formal framework for full evaluation is laid out.
- whether the comparison is full or partial: A partial comparison outlining an evaluation protocol because the repository lacks specific agricultural benchmark scores for the candidate models.
