# KTIR: Knowledge Tree-augmented Iterative Reasoning for Chinese Legal Multi-Choice Question Answering  
  
This repository contains the supplementary materials for the paper "Knowledge Tree-augmented Iterative Reasoning Method for Chinese Legal Multi-Choice Question Answering". The proposed KTIR method leverages hierarchical legal knowledge trees and iterative beam search to enhance deep reasoning in legal multi-choice question answering (LMCQA).  

To improve experimental reproducibility, we provide the following two key components in separate directories:  

📁 **Repository Structure**  
  
KTIR/  
├── datasets/ # (Raw dataset introduction)
├── knowledge_trees/ # Legal knowledge tree data (nodes & edges)  
└── README.md # This file  
  
📊 1. Datasets (datasets/)  
  
Experiments are conducted on two authoritative Chinese legal benchmarks:
JEC-QA: Largest Chinese legal MCQA benchmark ([GitHub](https://github.com/thunlp/jec-qa))  
DISC-Law-Eval: Real bar exam questions (2015–2022) ([GitHub](https://github.com/FudanDISC/DISC-LawLLM))  

🌳 2. Knowledge Tree Data (knowledge_trees/)  
  
The legal knowledge base consists of 18 concept trees, each rooted at a Chinese legal statute (e.g., Copyright Law, Patent Law). Each tree is provided as:  
nodes.csv  
edges.csv  
✅ Maximum tree depth: 8  
🔗 Source: Official legal textbooks endorsed by China’s Ministry of Justice (aligned with JEC-QA dataset)  
  
All node texts have been normalized for terminology consistency and manually validated by legal experts.  



📬 **Contact**  
  
For questions or collaboration:  
Mei Ma – gs.mma24@gzu.edu.cn  
Engineering Research Center of Text Computing & Cognitive Intelligence, Guizhou University, China  

    
✨ KTIR enables interpretable, knowledge-guided reasoning by fusing hierarchical legal knowledge with large language models.  

