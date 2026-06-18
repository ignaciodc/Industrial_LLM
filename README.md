![Python](https://img.shields.io/badge/Python-3.11-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![LLM](https://img.shields.io/badge/LLM-Llama%203.1%208B-orange)
![RAG](https://img.shields.io/badge/RAG-Enabled-red)
![Research](https://img.shields.io/badge/Research-Reproducible-brightgreen)

## Associated Publication

This repository accompanies the research paper:

Design and Evaluation of an Evidence-Aware RAG Pipeline for Industrial LLM Applications

Submitted to Expert Systems with Applications (Elsevier).

# Industrial LLM

Evidence-Aware RAG Pipeline for Reliable Industrial AI Systems

A modular architecture that combines planning, tool execution, retrieval, evidence construction, validation, and LLM reasoning to reduce hallucinations and improve reliability in industrial environments.

## Architecture

![Architecture](docs/fig.png)

## Key Contributions

- Multi-stage reasoning pipeline
- Tool-augmented analytics
- Evidence-aware response generation
- Validation layer for hallucination reduction
- Selective Retrieval-Augmented Generation (RAG)
- Fully local deployment

## Motivation

Industrial environments require reliable AI systems.

Traditional LLMs suffer from:
- Hallucinations
- Lack of traceability
- Poor integration with operational data

This project addresses these limitations through an evidence-aware architecture.

## Reproducibility

All experiments reported in the paper can be reproduced using:

python create_machine_db.py (only once)
python build_index.py (only once)
python main.py

## License
MIT License

