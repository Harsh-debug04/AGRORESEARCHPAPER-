# Jules Task Constraints

## Non-negotiable paper rules

* Do not preserve unsupported claims just because they already exist in the paper.
* README critique has priority over existing paper phrasing when the paper overclaims.
* Build the strongest defensible paper supported by repository evidence, not the strongest possible marketing narrative.
* Rewrite the fine-tuning dataset section carefully and honestly.
* Add a dataset statistics table only if the repository provides enough evidence to support it.
* Add a quality-control statement only if it can be defended from repo evidence.
* If multilingual evaluation is not actually present, frame multilingual capability as infrastructure support or future work rather than validated performance.
* If nitrogen reduction or farmer-impact claims are not supported by field evidence, explicitly narrow or remove them.
* Resolve author-name inconsistencies across the manuscript.
* Do not fabricate citations, ablation results, evaluation methodology details, deployment evidence, or comparative model results.

## LLM comparison study rules

* If the repository already contains evidence for multiple candidate open-source LLMs, use that evidence first.
* If the repository does not contain a complete comparison, do not invent scores.
* Any added model comparison must use a shared evaluation protocol and clearly state the compared setup (base / RAG / LoRA / RAG+LoRA).
* Add comparison tables and graphs only when backed by actual evaluation outputs or defensible computed results.
* The paper must explicitly explain which model performed best and why, or state honestly when the evidence supports only a partial comparison.
