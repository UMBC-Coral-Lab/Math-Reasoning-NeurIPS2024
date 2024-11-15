# SBI-RAG: Enhancing Math Word Problem Solving for Students through Schema-Based Instruction and Retrieval-Augmented Generation

This repository provides the official implementation for [SBI-RAG](https://arxiv.org/abs/2410.13293), which leverages Schema-Based Instruction (SBI) and Retrieval-Augmented Generation (RAG) to help students solve math word problems by guiding them through structured, schema-driven steps.

## Architecture

The SBI-RAG model architecture consists of four main components:
1. **Schema Classification**: A DistilBERT-based classifier predicts schemas and sub-categories for math word problems.
2. **Prompt Creation**: Generates structured prompts aligned with identified schemas.
3. **Context Retrieval**: Uses RAG to retrieve context to support problem-solving.
4. **Response Generation**: Employs Llama 3.1 to produce schema-driven, step-by-step solutions.

![SBI-RAG Architecture](Assets/SBI_RAG.jpg)

## Requirements

To install the required packages, run:

```bash
pip install -r requirements.txt
