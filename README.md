# 📚 RAG-Powered PDF Study Assistant

An intelligent full-stack application that transforms dense study materials and textbooks into concise summaries and targeted practice questions with answers, helping students grasp complex concepts faster.

---

## 🚀 Key Features

* **PDF Ingestion & Parsing:** Upload any study guide, textbook chapter, or research paper in PDF format.
* **Automated Summarization:** Generates structured, easy-to-digest summaries focusing on core takeaways.
* **Smart Q&A Generation:** Leverages Retrieval-Augmented Generation (RAG) to extract key concepts and create contextual review questions paired with detailed answers.
* **Student-Centric Design:** Built to bridge the gap between passive reading and active recall.

---

## 🛠️ Tech Stack

* **Backend:** Python, FastAPI / Flask *(update based on your stack)*
* **LLM & Orchestration:** LangChain / LlamaIndex, OpenAI / Hugging Face models *(update as applicable)*
* **Retrieval & Vector Search:** ChromaDB / FAISS / Pinecone with chunking strategies
* **Frontend:** React / Streamlit / Vanilla JS *(update as applicable)*

---

## ⚙️ Architecture & Workflow

1. **Document Loading:** The user uploads a PDF file via the interface.
2. **Text Extraction & Chunking:** The document is parsed, split into manageable semantic chunks, and embedded into a vector space.
3. **Retrieval (RAG):** Relevant context is retrieved based on queries or document sections.
4. **Generation:** The LLM processes the retrieved context to produce structured summaries and high-yield study questions with answers.

---

## 📂 Project Structure

```text
├── backend/
│   ├── app.py          # Main API endpoints / application logic
│   ├── rag_pipeline.py # Document loading, chunking, and retrieval logic
│   └── prompts.py      # System prompts for summarization and Q&A generation
├── frontend/
│   ├── src/            # UI components (Upload, Summary, Quiz views)
│   └── public/
├── requirements.txt    # Python dependencies
└── README.md
