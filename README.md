# RAG-Chat: AI-Powered PDF Q&A with LLMs  

**RAG-Chat** is a Retrieval-Augmented Generation (RAG) chatbot built using **Streamlit**, **Groq LLMs**, and **Nomic embeddings**. This application enables users to upload PDFs, extract information, and engage in contextual conversations with an AI-powered assistant.  

## Features  

- 📄 **Upload PDFs** and extract relevant information.  
- 🔍 **Retrieve answers** using FAISS vector search.  
- 🤖 **Engage in conversations** with an LLM-powered chatbot.  
- ⚙️ **Adjust chunk sizes** for optimized document retrieval.  
- 🧹 **Clear and restore chat history** with a single click.  

## Installation  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/yourusername/rag-chat.git
cd rag-chat
2️⃣ Create a Virtual Environment
bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate  # Windows
3️⃣ Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
4️⃣ Set API Keys
You need API keys for Groq and Nomic. Set them in your terminal:

bash
Copy
Edit
export GROQ_API_KEY="your_groq_api_key"
export NOMIC_API_KEY="your_nomic_api_key"
Alternatively, you can manually input them when running the application.

5️⃣ Run the Application
bash
Copy
Edit
streamlit run app.py
Usage
Upload a PDF document via the sidebar.
The document is split into chunks and embedded using Nomic embeddings.
A FAISS vector database is created for efficient similarity search.
Ask questions, and the chatbot retrieves relevant document chunks to generate accurate responses.
Tech Stack
Streamlit - UI for chatbot interaction
LangChain - Document processing and LLM integration
Groq LLMs - Provides natural language understanding
Nomic Embeddings - Converts text into vector representations
FAISS - Fast retrieval of relevant document chunks
Contributing
Contributions are welcome! Feel free to fork this repository, create a new branch, and submit a pull request
