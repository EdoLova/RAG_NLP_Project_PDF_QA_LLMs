# PDF QA with LLMs

This project implements a Retrieval-Augmented Generation (RAG) pipeline using a custom PDF knowledge base and large language models (LLMs). It focuses on building an LLM-based Q&A system for extracting answers from structured PDF content.

## Objectives
- Load a custom PDF knowledge base and split it into chunks.
- Build embeddings and a vector store for semantic search.
- Experiment with different chunk sizes and overlaps to observe their effect on answer quality.
- Answer targeted questions using RAG with LLMs.
- Generate a JSON report containing questions, answers, and reflections on retrieval quality.

## Tools and Libraries
- Python, PyTorch, Transformers, LangChain, Chroma
- SentenceTransformers for embeddings
- Matplotlib for visualizing document lengths
- PDF loader: PyPDFLoader

## Dataset
- `2024–25_Tottenham_Hotspur_F.C._season.pdf`: Custom knowledge base extracted from Wikipedia and articles.

## Main Results
- Generated answers for 3 questions regarding Tottenham Hotspur's 2024–25 season.
- Evaluated RAG performance with different chunk sizes (`100, 300, 500`) and overlaps (`20, 50, 100`).
- Reflections included in `rag_report_Edoardo_Lovato.json`.

## How to Run
1. Install required packages:

pip install langchain langchain-community pypdf faiss-cpu langchain-chroma bitsandbytes sentence-transformers transformers matplotlib


2. Place the PDF file in the same directory or update the file path in the script.

3. Run the Python script:

python PDF_QA_with_LLMs.py


4. The results will be saved as `rag_report_Edoardo_Lovato.json`.

## Author
Edoardo Lovato
Università di Padova – NLP (Natural Language Processing)
Academic Year 2024–2025
