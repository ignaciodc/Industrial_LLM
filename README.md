# Industrial LLM – An Evidence-Aware Architecture for Reliable Industrial AI

Evidence-Aware RAG Pipeline for Reliable Industrial AI Systems

A modular architecture that combines planning, tool execution, retrieval, evidence construction, validation, and LLM reasoning to reduce hallucinations and improve reliability in industrial environments.

![Python](https://img.shields.io/badge/Python-3.11-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![LLM](https://img.shields.io/badge/LLM-Llama%203.1%208B-orange)
![RAG](https://img.shields.io/badge/RAG-Enabled-red)
![Research](https://img.shields.io/badge/Research-Reproducible-brightgreen)


## Overview

Industrial LLM is an evidence-aware framework designed for industrial AI
applications where reliability, traceability and reproducibility are critical.

The framework combines:

- Tool execution
- Retrieval-Augmented Generation (RAG)
- Evidence construction
- Validation mechanisms
- LLM reasoning

to reduce hallucinations and improve decision quality.

## Motivation

Industrial environments require reliable AI systems.

Traditional LLMs suffer from:
- Hallucinations
- Lack of traceability
- Poor integration with operational data

This project addresses these limitations through an evidence-aware architecture.

## Associated Publication

This repository accompanies the research paper:

Design and Evaluation of an Evidence-Aware RAG Pipeline for Industrial LLM Applications

Submitted to Expert Systems with Applications (Elsevier).


## Key Contributions

- Multi-stage reasoning pipeline
- Tool-augmented analytics
- Evidence-aware response generation
- Validation layer for hallucination reduction
- Selective Retrieval-Augmented Generation (RAG)
- Fully local deployment

## Architecture

<p align="center">
  <a href="docs/fig1.png">
      <img src="docs/fig1.png" width="800">
  </a>
</p>



| Component | Purpose |
|------------|----------|
| Planner | Task decomposition |
| Tools | Data acquisition |
| RAG | Context retrieval |
| Evidence Validation | Verification |
| LLM | Final reasoning |


## Experimental Results

### Key Results

- 94.2% Grounded Accuracy
- 3.7% Hallucination Rate
- 95.6% Task Success Rate
- 96.4% Response Consistency

Compared with a standard LLM pipeline, the proposed evidence-aware architecture:

- Improves grounded accuracy by 19.4%
- Reduces hallucinations by 82.8%
- Improves task success by 19.3%
- Improves response consistency by 17.0%


| Metric | LLM-only | RAG | Tool-Aug. | Proposed | Gain vs LLM |
|----------|----------:|----------:|----------:|----------:|----------:|
| Grounded Accuracy ↑ | 74.8% | 82.7% | 88.4% | **94.2%** | **+19.4%** |
| Hallucination Rate ↓ | 21.5% | 13.8% | 8.9% | **3.7%** | **−82.8%** |
| Task Success Rate ↑ | 76.3% | 84.9% | 89.7% | **95.6%** | **+19.3%** |
| Response Consistency ↑ | 79.4% | 86.2% | 91.1% | **96.4%** | **+17.0%** |

*↑ Higher is better. ↓ Lower is better.*


## Repository Structure

├── planner/
├── tools/
├── rag/
├── validation/
├── experiments/
├── paper/
└── README.md

## Reproducibility

All experiments reported in the paper can be reproduced using:

python create_machine_db.py (only once)
python build_index.py (only once)
python main.py



## License
MIT License

