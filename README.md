# Evaluating Toxicity Propensity in Generative Language Models

This repository examines various large language models (LLMs) to produce toxic outputs when prompted. We assess the performance of three models—BLOOM 7B1, LLaMa 2 7B, and LLaMa 3 8B—using both automated toxicity detection tools and human evaluation protocols.

## Models Evaluated

- **BLOOM 7B1**
- **LLaMa 2 7B**
- **LLaMa 3 8B**

## Methodology

### Automated Toxicity Assessment

We utilize the [Detoxify](https://github.com/unitaryai/detoxify) library, specifically the Unitary Toxic BERT model fine-tuned on the Jigsaw dataset, to automatically evaluate the toxicity of model outputs. Detoxify provides probabilistic scores for various toxicity categories, including:

- **Toxicity**
- **Severe Toxicity**
- **Obscenity**
- **Threat**
- **Insult**
- **Identity Attack**

### Human Evaluation Protocol

We conduct human evaluations to capture nuances that automated tools may miss. The evaluation protocol is detailed in the `RQ1_3.ipynb` notebook, which includes:

- **Selection Criteria**: Guidelines for choosing a representative sample of model outputs for evaluation.
- **Annotation Guidelines**: Instructions for human annotators to assess toxicity levels and categories.
- **Data Analysis**: Methods for aggregating and interpreting human evaluation data.
