# Section Rewrite Map

## Title
- keep / rewrite / replace: Rewrite to "AgroTrack: A Retrieval-Augmented Generation Framework for Dynamic Crop Calendar Intelligence in Smallholder Agriculture"
- why: Removes "Hyper-Localized" which was unsupported by the 3-district pilot.

## Abstract
- key problems in current version: Claims 15-20% nitrogen reduction as real-world impact.
- what the final abstract must contain: Explicitly state the nitrogen reduction is a simulation and the pilot was a system load test. Mention the LLM comparison protocol.

## Introduction
- gap framing to add: Need for reliable, grounded agricultural advisory.
- unsupported claims to remove: Real-world agronomic impact of the pilot.
- contribution bullets to rewrite: Scope down contributions to system architecture, LoRA adaptation, and latency metrics. Add a bullet for the comparative evaluation framework.

## Related Work
- literature clusters to use: Citizen Science, Satellite Phenology, LLMs in Agriculture.
- weak comparisons to remove: Papers from 2026.
- citations to verify / replace: Ensure only pre-2025 citations are used.
- add subsection on open-source LLM selection: Yes, discussing the trade-offs of open-weight models for domain QA.

## Methodology
- architecture details to clarify: Two-tier ETL, RAG pipeline, LoRA fine-tuning.
- missing reproducibility details to add: None needed, keep existing strong descriptions.

## Fine-tuning Dataset Section
- rewrite plan: Full rewrite based on README.
- provenance wording to fix: Remove "generated", replace with manual curation.
- statistics table to add: Yes, Table 1 with dataset stats.
- quality-control paragraph to add: Yes, describing cross-checking.
- language-coverage wording: Predominantly English, multilingual as future work.

## Evaluation
- split into subsections: System Metrics, Hallucination, Agronomic Simulation, LLM Comparison Framework.
- LLM comparison study: Add a subsection detailing the framework to compare Mistral Large 2 with alternatives like Llama-3-70B, stating the current lack of domain-specific comparative data as a limitation.

## Hallucination / Groundedness
- methodology clarification needed: Specify it only tested banned substances.
- limitation language: Lack of formal rubric for broader agronomic correctness.

## Ablation
- whether LoRA-only can be supported: No.
- if not, how to rewrite honestly: Present RAG+LoRA as a combined pipeline and state missing LoRA-only as a limitation.

## Carbon Footprint
- how to reframe without overclaiming: Proof-of-concept IPCC Tier 1 feature.

## Discussion / Limitations
- limitations to state explicitly: Simulation-only agronomic impact, narrow hallucination test, lack of full LLM comparative data.

## Conclusion
- final tone and scope: Sober, evidence-based.
