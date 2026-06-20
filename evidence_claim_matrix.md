# Evidence Claim Matrix

| Claim ID | Claim | Where it appears | Evidence in repo | External verification available? | Status (Supported / Partially supported / Unsupported) | Final action |
|---|---|---|---|---|---|---|
| C1 | 1,200-farmer deployment | Table 4, Intro | Mentioned in text | No data on outcomes | Partially supported (as a latency test) | Scope to system load/latency only; remove agronomic impact claims. |
| C2 | <2% hallucination rate | 7.2 | Mentioned in text | No rubric/evaluator details | Partially supported (for narrow queries) | State explicitly it only applies to banned substance queries. |
| C3 | 15–20% nitrogen reduction | Abstract, 7.3 | Table 5 says 'Simulated Outcome' | No field data | Partially supported (as simulation) | Explicitly label as a simulation; remove real-world implication. |
| C4 | Multilingual capability (22 langs) | 1, 8.1 | Embedding model supports it | No evaluation data | Unsupported | Reframe as future work/infrastructure capability. |
| C5 | Carbon-footprint novelty | 5.4 | Equation 3 is IPCC Tier 1 | Yes, standard formula | Unsupported (as novelty) | Reframe as a standard proof-of-concept module. |
| C6 | Concurrent load (0% failure at 500) | 7.1 | Mentioned in text | No hardware specs | Partially supported | Keep as a system benchmark but acknowledge lack of hardware details in limitations. |
| C7 | Dataset provenance (12,000 generated) | 5.5 | README says manually curated | README | Supported (with README) | Rewrite to emphasize manual curation based on README. |
| C8 | Retrieval-performance | 7.1 | Latency reported | No relevance metrics | Partially supported (for latency) | Add limitation that relevance was not measured. |
| C9 | RAG+LoRA Ablation | 7.2 | Base, RAG, RAG+LoRA shown | No LoRA-only | Partially supported | Present as combined pipeline performance; state missing LoRA-only as limitation. |
