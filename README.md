# 🏢 Enterprise Knowledge Assistant

An AI-powered Enterprise Knowledge Assistant built using **Retrieval-Augmented Generation (RAG)**. It allows users to upload PDF documents and ask questions about their content using natural language.

Instead of manually searching through lengthy documents, users can get relevant answers based on the information available in the uploaded PDFs.

## 🚀 Project Overview

The Enterprise Knowledge Assistant uses RAG to retrieve relevant information from uploaded documents and generate concise, context-based answers.

It combines document processing, vector embeddings, similarity search, and a language model to provide an intelligent question-answering experience.

## ✨ Features

- 📄 Upload and process PDF documents.
- ✂️ Split documents into smaller text chunks.
- 🧠 Generate embeddings using Sentence Transformers.
- 🔍 Retrieve relevant information using FAISS vector search.
- 🤖 Generate answers using Google FLAN-T5 Base.
- 💬 Ask questions in natural language.
- 📚 Generate answers based only on the uploaded document context.
- ⚡ Reduce manual effort when searching through enterprise documents.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Streamlit | User interface |
| LangChain | RAG application framework |
| Hugging Face | Embeddings and language model |
| FLAN-T5 Base | Answer generation |
| Sentence Transformers | Text embeddings |
| FAISS | Vector database and similarity search |
| PyPDF | PDF document loading |

## 🏗️ Architecture

The application follows this RAG workflow:

1. **Document Upload:** Users upload PDF documents.
2. **Document Loading:** PyPDFLoader extracts text from PDFs.
3. **Text Splitting:** Documents are divided into chunks using RecursiveCharacterTextSplitter.
4. **Embedding Generation:** Sentence Transformers converts text chunks into vector embeddings.
5. **Vector Storage:** FAISS stores the embeddings for efficient similarity search.
6. **Information Retrieval:** Relevant chunks are retrieved based on the user's question.
7. **Answer Generation:** FLAN-T5 generates an answer using the retrieved context.

## 📂 Project Structure

```text
Enterprise-Knowledge-Assistant/
│
├── app.py
├── rag_pipeline.py
├── requirements.txt
├── Enterprise_Demo_Document.pdf
├── README.md
└── .gitignore
```

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/SravaniVeeramreddy/Enterprise-Knowledge-Assistant.git
```

### 2. Navigate to the project directory

```bash
cd Enterprise-Knowledge-Assistant
```

### 3. Create a virtual environment

```bash
python -m venv venv
```

### 4. Activate the virtual environment

For Windows:

```bash
venv\Scripts\activate
```

### 5. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 6. Run the application

```bash
streamlit run app.py
```

The application will open in your browser.

## 🧪 Example Questions

You can ask questions such as:

- How many annual leave days are provided to employees?
- What is the maternity leave policy?
- How often should employees change their passwords?
- What is the company's work-from-home policy?
- What is the travel allowance for employees?

The assistant retrieves relevant information from the uploaded PDF and generates answers based on the document.

## 🎯 Project Objective

The main objective of this project is to demonstrate how Retrieval-Augmented Generation can be used to build an intelligent document-based question-answering system for enterprise knowledge management.

## 🔮 Future Enhancements

- Support for multiple document formats.
- Multi-document question answering.
- Chat history and conversation memory.
- Improved retrieval using advanced embedding models.
- Source citations for generated answers.
- Deployment using Streamlit Community Cloud.

## 👩‍💻 Author
V. Venkata Sravani
**Developed as an AI-powered Enterprise Knowledge Assistant project.**

## 📌 GitHub Repository

[Enterprise Knowledge Assistant](https://github.com/SravaniVeeramreddy/Enterprise-Knowledge-Assistant)
