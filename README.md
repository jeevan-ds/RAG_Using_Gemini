# RAG_Using_Gemini
Implemented a Retrieval-Augmented Generation system leveraging Google Gemini, FAISS vector search, and PDF embeddings to extract accurate, context-aware insights from financial reports
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/36215cdb-77dd-477b-aa98-8ea71fff9cf1" />

#  RAG Using Gemini on Financial PDF (Sharekhan – Investor Eye)

##  Project Overview
This project implements an **end-to-end Retrieval-Augmented Generation (RAG)** system using **Google Gemini**, **FAISS vector database**, and a **financial PDF document (Sharekhan – Investor Eye)**.  

The system allows users to ask natural language questions and receive **context-aware, accurate answers grounded in the source document**, overcoming the limitation of LLMs not having direct access to private or external documents.

---

##  Problem Statement
Financial reports are lengthy, complex, and time-consuming to analyze manually. Traditional LLMs may hallucinate or provide generic answers without understanding document-specific context.

**Objective:**  
Build a system that can:
- Understand financial PDFs
- Retrieve relevant information efficiently
- Generate precise, context-grounded answers

---

##  Solution Approach (RAG Pipeline)

1. **PDF Ingestion**
   - Load and extract text from the Sharekhan Investor Eye PDF using `PyPDF2`

2. **Text Chunking**
   - Split extracted text into smaller, semantically meaningful chunks

3. **Embedding Generation**
   - Convert text chunks into dense vector embeddings

4. **Vector Storage**
   - Store embeddings in a **FAISS** vector database for fast similarity search

5. **Query Processing**
   - Convert user queries into embeddings
   - Retrieve top-k relevant chunks from FAISS

6. **Answer Generation**
   - Pass retrieved context along with the user query to **Google Gemini**
   - Generate accurate, document-grounded responses

---

## Tech Stack

- **Language:** Python  
- **LLM:** Google Gemini  
- **Vector Database:** FAISS  
- **PDF Processing:** PyPDF2  
- **Embeddings:** LLM-based / Sentence embeddings  
- **Environment:** Jupyter Notebook  

---

