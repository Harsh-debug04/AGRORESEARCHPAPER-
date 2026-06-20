# LLM Comparison Plan

## Candidate models
| Model | Size | Open-source/open-weight? | Why included | Repo evidence / existing use |
|---|---:|---|---|---|
| Mistral Large 2 | 123B | Open-weight | Used as the main model in the paper | Main focus of the paper |
| Llama-3-70B | 70B | Open-weight | Comparable alternative for NLP benchmarks | Mentioned in Figure 3 of the original paper |
| GPT-4o-mini | Unknown | Closed | Included as a generic baseline | Mentioned in Figure 3 of the original paper (but we will remove or heavily caveat this since the focus is open-source) |

*Note: Since the paper only cites Mistral Large 2 and Llama-3-70B (and GPT-4o-mini as an estimate), and the Q1 Review Report criticizes using generic NLP benchmarks instead of agronomic tasks, the repo does NOT contain evidence of an actual comparative LLM study on the AgroTrack task itself. Therefore, we cannot fabricate a comparative study. We will construct a "comparative benchmarking protocol + partial results + limitation statement" as mandated by the instructions.*

## Evaluation goal
- To determine the most suitable open-source LLM for the AgroTrack agricultural advisory task, focusing on agronomic QA, hallucination resistance, and latency.

## Shared evaluation setup
- **Condition:** Base LLM vs RAG vs RAG+LoRA (where supported).
- **Task:** Agronomic QA on 500 adversarial queries (banned substances) and a proposed wider agronomic QA set.
- **Limitation:** The current repo only has data for Mistral Large 2 on the hallucination task. The comparison will outline the protocol and state that full multi-model agronomic evaluation is pending.

## Metrics
- Hallucination rate (currently only measured for Mistral Large 2 on adversarial queries)
- Retrieval latency (system level)
- End-to-end response latency

## Expected output artifacts
- A dedicated subsection outlining the comparative evaluation framework.
- A limitation statement acknowledging that full comparative results across Llama-3 and Mistral on the specific agronomic task are future work.
