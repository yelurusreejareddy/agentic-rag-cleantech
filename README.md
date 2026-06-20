# agentic-rag-cleantech

LangChain agent for question answering over cleantech media articles,
comparing a Base agent against an Extended agent with additional tools.

## Files Included

- Sreejareddyyeluru_finalproject.ipynb - end-to-end notebook with both agents
- Finalprojectreport.pdf - full project report
- cleantech_rag_evaluation_data_2024-09-20.csv - 23-question evaluation set
- CleanTech-50answers.txt - 50-question extended evaluation set
- part1_agent_answers.csv - Base agent outputs
- part2_advanced_results.csv - Extended agent outputs
- Final_Part3_Evaluation.csv - BLEU, ROUGE, BERTScore comparison results

Note: Main dataset (Cleantech Media Dataset by Anacode, 101MB) not included due to size.

## Techniques Used

- ChromaDB vector store with MiniLM embeddings for document retrieval
- Base agent - retriever tool + summarizer tool
- Extended agent - adds Semantic Scholar paper search + chain-of-thought reasoning
- Evaluation using BLEU, ROUGE, and BERTScore

## Libraries

pandas, numpy, LangChain, ChromaDB, SentenceTransformers, OpenAI API (GPT-4o-mini),
Semantic Scholar API, evaluate, rouge-score, bert-score

## Goal

To explore how adding tools and reasoning steps to a RAG agent improves answer
quality on real-world cleantech research questions.
