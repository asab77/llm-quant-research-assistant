# 🤖 LLM-Powered Quant Research Assistant

An AI assistant for financial research that answers natural language questions about **10-K filings**, **earnings reports**, and **market news**. Uses Retrieval-Augmented Generation (RAG) to provide accurate, source-grounded responses.

---

## 🚀 Demo

<div align="center">
  <img src="assets/demo.gif" alt="Demo" width="700"/>
  <br/>
  <em>Answering financial research queries with source citations</em>
</div>

---

## 🧠 Features

- 📄 **Document Ingestion:** Upload PDFs of 10-K filings or earnings reports.
- 🔍 **Vector Search:** Retrieve most relevant document chunks using embeddings.
- 💬 **Natural Language Q&A:** Ask questions in plain English, get answers with citations.
- 🧮 **RAG Pipeline:** Combines retrieval with LLMs for accurate, grounded responses.

---

## 🛠 Tech Stack

- **Python 3.10+**
- `LangChain` or `LlamaIndex` for RAG
- Hugging Face `transformers` for embeddings
- `FAISS` or `Chroma` for vector storage
- `PyMuPDF` or `pdfminer` for PDF parsing
- `Streamlit` for chat interface

---

## 📁 Project Structure

```
quant-llm-assistant/
│
├── data/
│   ├── filings/                # PDF financial reports
│
├── src/
│   ├── parse_pdfs.py           # Extract text from PDFs
│   ├── embed_store.py          # Create embeddings and store in FAISS
│   ├── rag_query.py            # Retrieve relevant chunks and query LLM
│
├── app.py                      # Streamlit chat interface
├── requirements.txt
├── README.md
└── assets/                     # Demo GIFs or screenshots
```

---

## 🧪 How It Works

1. **Parse PDFs** of financial documents.
2. **Chunk text** into overlapping segments.
3. Generate **embeddings** for each chunk.
4. Store in **FAISS** vector database.
5. For a user query:
   - Retrieve top N relevant chunks.
   - Pass chunks + query to LLM.
   - Return answer with **source citations**.

---

## 📦 Installation

```bash
git clone https://github.com/yourusername/quant-llm-assistant.git
cd quant-llm-assistant
pip install -r requirements.txt
```

---

## ▶️ Run the App

```bash
streamlit run app.py
```

---

## 📈 Model Options

| Model           | Type            | Notes                                |
|-----------------|-----------------|---------------------------------------|
| Llama 3 / Mistral| Open-Source LLM | Use with LangChain for RAG            |
| OpenAI GPT-4    | API-based LLM   | Higher accuracy, paid API             |

---

## 🧠 Future Work

- Integrate **real-time news APIs**.
- Support multi-document querying.
- Add **fine-tuning** for financial domain.

---

## 📄 License

MIT License

---

## 🤝 Let's Connect

- Created by **Aria Saboonchi Lilabady**  
- [LinkedIn](https://linkedin.com/in/...) | [Portfolio](https://your-portfolio.com)
