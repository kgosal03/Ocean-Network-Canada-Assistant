
## 📌 Overview
The Ocean Network Canada AI Assistant is a conversational system designed to provide natural language access to **Ocean Networks Canada’s Oceans 3.0 data archive**.  
It enables researchers, educators, Indigenous communities, policymakers, and students to query oceanographic datasets in plain English and receive accurate, cited responses with visualizations.

The system leverages a **RAG (Retrieval-Augmented Generation) pipeline** to combine live sensor data, curated knowledge bases, and research documents with large language model capabilities.  
This ensures factual, contextually relevant, and transparent answers.

![1](/screenshots/1.png)
---

## ✨ Key Features
- **Natural Language Queries** – Ask questions like *“What’s the water temperature in Cambridge Bay?”* and receive clear, cited responses.  
- **RAG Pipeline** – Combines embeddings, vector retrieval, re-ranking, and LLM generation to improve accuracy.  
- **Accuracy & Benchmarks** – Achieved **96% accuracy** in benchmark testing with <2s average latency.  
- **Data Transparency** – Every response includes full source citations, raw data links, and metadata.  
- **User Personalization** – Adapts answers for different user roles (students, researchers, educators).  
- **Admin Dashboard** – Allows ONC staff to upload documents, review queries, and manage knowledge content.  
- **Indigenous Knowledge Integration** – Supports culturally respectful representation alongside scientific data.

---

## ⚙️ System Architecture
1. **User Input Layer** – Accepts plain-language queries.  
2. **Query Processing** – Intent recognition, entity extraction, query expansion.  
3. **Embedding & Vectorization** – Converts queries into semantic vectors.  
4. **Retrieval & Ranking** – Searches ChromaDB/FAISS vector store and re-ranks results.  
5. **Context Processing** – Compresses, validates, and prepares retrieved content.  
6. **Generation Phase** – Produces answers using fine-tuned LLaMA/GPT-based models.  
7. **Response Output** – Returns natural language answers with visualizations and citations.  
8. **Feedback Loop** – Improves system continuously based on user input.

---

## 🛠️ Technology Stack
- **Frontend**: Next.js / React.js, Tailwind CSS  
- **Backend**: FastAPI (Python)  
- **Database**: PostgreSQL + Vector Database (ChromaDB)  
- **LLM**: LLaMA 3.1 (via Groq)  