# Retrieval-Augmented Generation (RAG) QA System

## Overview
This project implements a Retrieval-Augmented Generation (RAG) system to enable intelligent querying of a PDF document (in this case, my CV) using natural language.  
By combining semantic search with a large language model (LLM), the system generates accurate, document-grounded answers without requiring model retraining.

---

## Key Features
- **Document Ingestion & Chunking** – PDF split into smaller sections for efficient processing.  
- **Semantic Embeddings** – Created vector representations of text using embedding models.  
- **Vector Database (FAISS)** – Indexed and stored embeddings for fast semantic retrieval.  
- **LLM Integration** – Used a transformer model (Flan-T5) to generate answers based on retrieved context.  
- **End-to-End QA** – User asks a question → relevant chunks retrieved → LLM generates grounded response.

---

## Workflow
1. Upload the PDF document.  
2. Split the text into manageable chunks.  
3. Generate embeddings and store them in FAISS.  
4. Pass user questions through the RAG pipeline.  
5. Retrieve relevant context and generate natural language answers using the LLM.  

---

## Tools & Technologies
- Python  
- Hugging Face Transformers (Flan-T5)  
- FAISS for vector storage & search  
- Semantic Embedding Models  

---

## Outcome
- Built a working document-based QA system that can accurately answer questions from a CV.  
- Demonstrated the practical value of combining information retrieval with generative AI.  
- Hands-on experience with semantic search, embeddings, and RAG pipelines.

---

## Example Usage
**Input:**  
`Summarize the key points of this document in a paragraph of 200 words.`  

**Output:**  
`Skilled in analyzing large datasets, identifying trends, and providing actionable insights to support business decision-making. Eager to contribute analytical and problem-solving skills to dynamic, data-driven teams.`  

---


