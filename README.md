# Financial-Analysis-Agent-Hackathon
Team: O_Chamchuri-2

Ethical Finance Hackathon: The "Greeny" Agent
This repository contains the source code for the Greeny Agent, our entry for the SCB-10X Ethical Finance Hackathon.
Agent Design: The "Greeny" Protocol
The Greeny Agent is an intelligent system designed for accuracy, efficiency, and ethical alignment. Instead of relying on a single, monolithic model, Greeny uses a modular, tool-augmented architecture to deliver precise and auditable financial analysis.
Our design is built on three core pillars:
1. Thai-Specialized Core
We use KBTG-Labs/THaLLE-0.1-7B-fa as our foundation. This model is already an expert in the Thai language, providing a high-performance and culturally aware base without the risks of fine-tuning.
2. Intelligent Task Routing & Chain-of-Thought (CoT)
Greeny first classifies each query into one of three types: Stock Prediction, Ethical Scenario, or General MCQ. It then generates a custom prompt for that specific task, forcing the model to reason step-by-step (Chain-of-Thought) before providing an answer. This significantly boosts accuracy and transparency.
3. Expert Pre-Processing Tools
Before the LLM sees a query, our automated tools provide structured analysis:
Quantitative Analyzer: For stock predictions, this tool calculates technical momentum and analyzes social media sentiment, feeding a concise summary to the LLM.
Compliance RAG Agent: For ethical questions, this tool uses Retrieval-Augmented Generation (RAG) to find and inject relevant BOT/SEC principles directly into the prompt. This ensures all ethical reasoning is grounded in verifiable compliance rules.
