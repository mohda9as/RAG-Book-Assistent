# 📚 RAG Book Assistant

**An AI powered Retrieval Augmented Generation system that helps users explore book content and generate context aware answers from documents.**

RAG Book Assistant combines document processing, vector search, and language model capabilities to make information retrieval more useful and efficient. The project explores how AI systems can retrieve relevant information from a document collection before generating answers.

##  Key Features

📄 **Document Processing:** Load and process documents for retrieval.

🧠 **Vector Storage:** Store document representations in a vector database using ChromaDB.

🔍 **Semantic Retrieval:** Retrieve relevant information based on a user's query.

🔄 **Multiple Retrieval Strategies:** Explore Multi Query Retrieval and Maximum Marginal Relevance (MMR).

🤖 **Context Aware Responses:** Use retrieved document content to support answer generation.

💾 **Persistent Storage:** Keep vector database data available for reuse.

## 🛠️ Tech Stack

**Language:** Python

**AI Architecture:** Retrieval Augmented Generation (RAG)

**Vector Database:** ChromaDB

**Core Concepts:** Document Loading, Text Chunking, Embeddings, Semantic Search, Context Retrieval

**Dependencies:** Python libraries listed in `requirements.txt`

## 🏗️ System Architecture

```text
Documents
    ↓
Document Loading
    ↓
Text Splitting
    ↓
Embedding Generation
    ↓
ChromaDB Vector Store
    ↓
Relevant Context Retrieval
    ↓
Language Model
    ↓
Context Aware Answer
```

## 📁 Project Structure

```text
RAG-Book-Assistent/
│
├── app.py
├── main.py
├── create_database.py
├── requirements.txt
│
├── document loaders/
│   ├── GRU.pdf
│   ├── deeplearning.pdf
│   ├── notes.txt
│   ├── page.py
│   ├── pdf.py
│   └── test.py
│
├── retrievers/
│   ├── arixv.py
│   ├── mmr.py
│   └── multiquery.py
│
├── vector store/
│   └── DB.py
│
└── chroma_db/
    └── Persistent vector database files
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/mohda9as/RAG-Book-Assistent.git
cd RAG-Book-Assistent
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

Activate the environment on Windows:

```bash
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

If the project requires API credentials, configure them using the environment variable names expected by the application.

Keep all API keys and secrets private. Never commit them to the repository.

### 5. Run the Application

Choose the entry point that matches your implementation.

For a Streamlit application configured through `app.py`:

```bash
streamlit run app.py
```

For a standard Python script, run the appropriate entry point using Python.

## 🧠 How Retrieval Augmented Generation Works

**1. Document Loading**

The system reads source documents and prepares their content for processing.

**2. Text Splitting**

Large documents can be divided into smaller chunks to support retrieval of relevant passages.

**3. Embedding Generation**

Text chunks are converted into vector representations for similarity based search.

**4. Vector Storage**

The vector representations are stored in ChromaDB for later retrieval.

**5. Context Retrieval**

When a user submits a question, the system searches for relevant information from the stored document collection.

**6. Answer Generation**

The retrieved context is used to support the generation of a relevant response.

## 🔎 Retrieval Techniques

**Multi Query Retrieval**

Explores generating multiple query variations to improve the chances of finding relevant information.

**Maximum Marginal Relevance (MMR)**

Balances relevance and diversity when selecting retrieved information, helping reduce redundant results.

## 🚀 Future Enhancements

📌 Add source citations and document references to generated answers.

📌 Improve retrieval accuracy and response quality.

📌 Build a polished and interactive user interface.

📌 Support additional document formats.

📌 Deploy the application for public access.

## 👨‍💻 Author

**Mohd Anas**

GitHub: [@mohda9as](https://github.com/mohda9as)

⭐ If you find this project interesting, consider starring the repository.

