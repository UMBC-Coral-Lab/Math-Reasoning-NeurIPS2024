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
'''
Environment Setup
To set up the environment:

Clone this repository.
Install dependencies from requirements.txt.
Download the datasets (details below).
Ensure access to Google Colab or a local setup with GPU support.
Data Preparation
This project utilizes two main datasets:

Schema-Based Instruction (SBI) Dataset: A custom dataset of 360 labeled math word problems categorized across six schema sub-categories.
GSM8K Dataset: A collection of 8.5K grade school math word problems for evaluation.
Note: The custom SBI dataset can be found in the repository, and GSM8K is openly accessible here.

Training
To train the Schema Classifier model, access the provided Colab notebook. You can experiment with different hyperparameters in the notebook’s configuration section.

Pre-trained Models
Pre-trained models are available for download here. These models were trained on DistilBERT using default hyperparameters.

Evaluation
SBI-RAG is evaluated based on reasoning clarity and correctness. Below is an overview of its performance:

Model	Top 1 Accuracy	Reasoning Score (SBI-RAG)
SBI-RAG	85%	0.588
GPT-4	N/A	0.491
GPT-3.5 Turbo	N/A	0.290
For detailed evaluation, refer to evaluation_results.md.

Contributing
This repository follows the MIT License. We welcome contributions! To contribute, fork the repository, create a new branch, and submit a pull request.
