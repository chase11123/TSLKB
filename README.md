# KTIR: Knowledge Tree-augmented Iterative Reasoning for Chinese Legal Multi-Choice Question Answering

This repository contains the supplementary materials for the paper "A Knowledge Tree-augmented Iterative Reasoning Method for Chinese Legal Multi-Choice Question Answering", submitted to ICASSP 2026. The proposed KTIR method leverages hierarchical legal knowledge trees and iterative beam search to enhance deep reasoning in legal multi-choice question answering (LMCQA).

To address reviewer concerns regarding reproducibility, we provide the following four key components in separate directories:

📁 Repository Structure

KTIR/
├── hyperparameters/ # Hyperparameter selection reports with experimental results
├── llm_prompts/ # LLM prompt implementations (Python files)
├── knowledge_trees/ # Legal knowledge tree data (nodes & edges)
└── README.md # This file

🧪 1. Hyperparameter Study (hyperparameters/)

We conducted systematic ablation studies to select two critical hyperparameters:
(1) Candidate Chain Number Selection
(2) Relevance Score Threshold Selection



💬 2. LLM Prompts (llm_prompts/)

This directory contains two Python files that encapsulate the exact prompts used during inference:
llm_evaluation.py:
Implements the prompt for assessing the relevance of a knowledge chain w.r.t. a given legal question. 
llm_generation.py:
Defines the prompt for final answer generation, which combines the original question and the top-relevant knowledge chains retrieved by KTIR.


🌳 3. Knowledge Tree Data (knowledge_trees/)

The legal knowledge base consists of 18 concept trees, each rooted at a Chinese legal statute (e.g., Copyright Law, Patent Law). Each tree is provided as:
nodes.csv
edges.csv
✅ Maximum tree depth: 8
🔗 Source: Official legal textbooks endorsed by China’s Ministry of Justice (aligned with JEC-QA dataset)

All node texts have been normalized for terminology consistency and manually validated by legal experts.


📊 Evaluation Datasets

Experiments conducted on:
JEC-QA: Largest Chinese legal MCQA benchmark ([GitHub](https://github.com/thunlp/jec-qa))
DISC-Law-Eval: Real bar exam questions (2015–2022) ([GitHub](https://github.com/FudanDISC/DISC-LawLLM))

We do not redistribute these datasets. Please obtain them from official sources.



📬 Contact

For questions or collaboration:
Mei Ma – gs.mma24@gzu.edu.cn
Engineering Research Center of Text Computing & Cognitive Intelligence, Guizhou University, China

✨ KTIR enables interpretable, knowledge-guided reasoning by fusing structured legal ontologies with large language models.

