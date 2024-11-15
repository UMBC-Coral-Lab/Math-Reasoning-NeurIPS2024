# Evaluation Results for SBI-RAG

This document provides detailed evaluation results for the SBI-RAG model, which enhances math word problem-solving skills using Schema-Based Instruction (SBI) and Retrieval-Augmented Generation (RAG).

## Overview of Evaluation Metrics

SBI-RAG has been evaluated based on reasoning clarity and correctness compared to baseline models using the LLM-as-a-Judge approach. This approach leverages a large language model to score responses based on criteria such as clarity, logical progression, and completeness.

| Model          | Reasoning Score (SBI-RAG) |
|----------------|---------------------------|
| SBI-RAG        | 0.588                     |
| GPT-4          | 0.491                     |
| GPT-3.5 Turbo  | 0.290                     |

### LLM-as-a-Judge Results

The LLM-as-a-Judge approach is a reference-free evaluation method that uses large language models to objectively score the quality of generated responses without requiring human evaluation. The scoring criteria include:

- **Clarity**: Measures how clearly the response conveys the solution.
- **Logical Progression**: Assesses whether each step follows logically from the previous one.
- **Completeness**: Ensures that all aspects of the problem are fully addressed in the response.

Using these criteria, each model’s responses were rated on a scale of 0 to 10, with SBI-RAG consistently outperforming GPT-4 and GPT-3.5 Turbo in terms of reasoning quality.

### Key Findings

- **Schema-Based Advantage**: SBI-RAG’s schema-driven prompts led to higher scores in clarity, logical progression, and completeness compared to the baseline models.
- **Consistency in Reasoning**: SBI-RAG produced more coherent and logically structured explanations, which are beneficial for educational applications.
- **Educational Effectiveness**: The use of schema-based instruction aligns well with step-by-step problem-solving, allowing for greater interpretability and reliability in responses.

## Statistical Significance

A paired sample t-test was conducted to assess the statistical significance of SBI-RAG's performance over the baseline models:

- **SBI-RAG vs. GPT-4**: Significant at p < 0.05.
- **SBI-RAG vs. GPT-3.5 Turbo**: Significant at p < 0.01.

These results confirm that SBI-RAG’s schema-based approach significantly enhances reasoning quality over traditional LLM responses without schema guidance.

## Conclusion

The SBI-RAG model demonstrates a substantial improvement in structured reasoning for math word problems, as validated by the LLM-as-a-Judge scoring. These findings suggest that schema-based frameworks may provide meaningful educational benefits, particularly in contexts requiring logical, step-by-step problem-solving.

For further details on the implementation and training methodology, please refer to the main [README](README.md) file.
