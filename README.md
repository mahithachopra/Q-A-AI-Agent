# Q-A-AI-Agent
# 📄 Chat with PDF using Google Gemini

This is a Streamlit-based application that allows users to upload one or more PDF documents and ask questions about their content. The application uses Google's **Gemini** model for embeddings and response generation, making PDF document interaction smarter and more intuitive.

---

## 🚀 Features

- 📁 Upload and process multiple PDF files
- 🧠 Uses **LangChain** and **Google Generative AI (Gemini)** for understanding documents
- 💬 Asks questions and gets context-aware answers from uploaded PDFs
- 🔍 Semantic search with vector embeddings using **FAISS**
- 🌐 Runs locally with a simple Streamlit interface

---

## 🛠️ Tech Stack

- Python 🐍
- Streamlit 📊
- Google Generative AI (Gemini) 🤖
- LangChain 🔗
- FAISS 🔎
- PyPDF2 📄
- dotenv 🔐

---

## Create and activate a virtual environment:
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate

## Install the required packages:
pip install -r requirements.txt

## Set up your environment variables:
Create a .env file in the root directory and add your Google API key:
GOOGLE_API_KEY=your_api_key_here

## ▶️ Running the Ap
streamlit run app.py

## 🧠 How It Works
- PDF Upload: Users upload PDF files via the sidebar.

- Text Extraction: PyPDF2 extracts the text content.

- Text Chunking: Text is split into chunks using RecursiveCharacterTextSplitter.

- Vector Store Creation: Chunks are embedded using Google Gemini and stored in a FAISS index.

- Question Answering: User questions are semantically matched with the text chunks and answered using ChatGoogleGenerativeAI.

## 📂 Project Structure
.
├── app.py
├── .env
├── requirements.txt
└── faiss_index/


## 📌 Requirements
Make sure to include these packages in requirements.txt:
streamlit
langchain
google-generativeai
chromadb
PyPDF2
faiss-cpu
python-dotenv

## 💡 Use Case
- Ideal for students, researchers, or professionals who want to:

- Analyze research papers

- Extract information from large PDFs

- Get instant answers from documentation

## 📬 Contact
For issues or questions, feel free to contact mahithachopra.lankapalli@gmail.com












