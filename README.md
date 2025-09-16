
# 📄 Summarize Private Documents Using RAG, LangChain, and LLMs

**Repository Description:**
This repository contains a complete workflow to build a **Retrieval-Augmented Generation (RAG) pipeline** for summarizing and querying private documents using **LangChain, IBM Watsonx AI, HuggingFace embeddings, and ChromaDB**.
It enables you to interact with sensitive documents securely without uploading them to public LLMs.

---

## 🚀 Features

* Load and process private text documents
* Split large documents into manageable chunks
* Generate embeddings using **HuggingFace models**
* Store and retrieve embeddings with **ChromaDB**
* Build a **RetrievalQA chain** for question-answering
* Add **conversational memory** to maintain context
* Integrate with **IBM Watsonx LLM** via LangChain
* Extend functionality with prompt templates and agent-based interactions

---

## 🛠️ Tech Stack

* **Python 3.9+**
* **LangChain** – framework for building LLM applications
* **IBM Watsonx AI** – foundation model integration
* **Transformers & HuggingFace Hub** – embeddings and language models
* **Sentence Transformers** – semantic embeddings
* **ChromaDB** – vector database for retrieval
* **PyTorch** – backend for embeddings
* **wget** – to fetch documents

---

## 📂 Project Structure

```
📦 Summarize-Private-Documents
 ┣ 📜 README.md              # Project documentation
 ┣ 📜 notebook.ipynb         # Jupyter Notebook (main code)
 ┗ 📜 requirements.txt       # Dependencies
```

---

## ⚙️ Installation

Clone this repo and install dependencies:

```bash
git clone https://github.com/your-username/Summarize-Private-Documents.git
cd Summarize-Private-Documents

pip install -r requirements.txt
```

Or install inside the notebook:

```python
!pip install "ibm-watsonx-ai==0.2.6"
!pip install "langchain==0.1.16"
!pip install "langchain-ibm==0.1.4"
!pip install "transformers==4.41.2"
!pip install "huggingface-hub==0.23.4"
!pip install "sentence-transformers==2.5.1"
!pip install "chromadb"
!pip install "wget==3.2"
```

---

## ▶️ Usage

1. Place your private document (e.g., `companyPolicies.txt`) in the project folder.
2. Run the notebook `Summarize_Private_Documents.ipynb`.
3. The pipeline will:

   * Load and split documents
   * Generate embeddings
   * Store/retrieve chunks from ChromaDB
   * Use Watsonx LLM + LangChain for summarization and Q\&A

Example:

```python
query = "Summarize the company policies on leave."
response = qa_chain.run(query)
print(response)
```

---

## 📊 Example Output

* **Input:** Long private text file (policies, manuals, etc.)
* **Output:** Concise summaries, answers to queries, context-aware conversations

---

## 🤝 Contributing

Contributions are welcome!

* Fork the repo
* Create a feature branch
* Submit a Pull Request

---

## 👨‍💻 Author

**Taraka Nadh (Chinna Pandu)**
💼 Aspiring Data Analyst | AIML Engineer | Full-Stack Python Developer
