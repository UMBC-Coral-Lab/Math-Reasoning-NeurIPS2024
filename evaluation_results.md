# Evaluation Results for SBI-RAG

This document provides detailed evaluation results for the SBI-RAG model, which enhances math word problem-solving skills using Schema-Based Instruction (SBI) and Retrieval-Augmented Generation (RAG).

## Overview of Evaluation Metrics

SBI-RAG has been evaluated based on reasoning clarity and correctness compared to baseline models. The metrics below indicate how well each model performed in terms of generating structured, schema-driven responses.

| Model          | Top 1 Accuracy | Reasoning Score (SBI-RAG) |
|----------------|----------------|---------------------------|
| SBI-RAG        | 85%            | 0.588                     |
| GPT-4          | N/A            | 0.491                     |
| GPT-3.5 Turbo  | N/A            | 0.290                     |

### Metric Descriptions

- **Top 1 Accuracy**: Measures the percentage of correct answers produced by the model on the first attempt.
- **Reasoning Score (SBI-RAG)**: A custom metric designed to evaluate the quality of schema-based reasoning in the generated solutions. This score assesses clarity, logical progression, and completeness of reasoning in solving math word problems.

## Evaluation Methodology

The evaluation methodology for SBI-RAG includes:

1. **Schema-Based Classification**: Using a DistilBERT classifier, math word problems are categorized according to schema types (e.g., additive and multiplicative structures).
2. **Step-by-Step Reasoning**: The Llama 3.1 language model generates solutions guided by schema-specific prompts, ensuring structured reasoning.
3. **Comparison Against Baselines**: SBI-RAG’s performance is compared with GPT-4 and GPT-3.5 Turbo in terms of reasoning score.

### Key Findings

- SBI-RAG achieved the highest Reasoning Score, reflecting its effectiveness in providing structured, schema-based solutions.
- Comparisons with GPT-4 and GPT-3.5 Turbo demonstrate that SBI-RAG produces more logically coherent and educationally useful explanations.
- The custom Reasoning Score metric confirms that schema-guided approaches improve clarity and comprehension in math word problem-solving.

## Statistical Significance

A paired sample t-test was conducted to determine the statistical significance of SBI-RAG's Reasoning Score over the baseline models:

- **SBI-RAG vs. GPT-4**: Significant at p < 0.05.
- **SBI-RAG vs. GPT-3.5 Turbo**: Significant at p < 0.01.

These results confirm that SBI-RAG’s schema-based approach significantly enhances the quality of reasoning over traditional LLM approaches without schema guidance.

## Conclusion

SBI-RAG demonstrates a significant improvement in structured reasoning for math word problems. These results suggest that schema-based frameworks may provide educational benefits in settings where logical, step-by-step reasoning is essential.

For further details on the implementation and training methodology, please refer to the main [README](README.md) file.
