# RAG-Chat: AI-Powered PDF Q&A with LLMs  

This project implements a **Retrieval-Augmented Generation (RAG)** chatbot using **Streamlit**, **Groq LLMs**, and **Nomic embeddings**. The chatbot enables users to upload PDFs, extract relevant information, and engage in meaningful conversations with an AI assistant.  

## Table of Contents  
- [Installation](#installation)  
- [Dataset Processing](#dataset-processing)  
- [Usage](#usage)  
- [Models Used](#models-used)  
- [Embedding and Vector Search](#embedding-and-vector-search)  
- [Chatbot Functionality](#chatbot-functionality)  
- [Evaluation](#evaluation)  
- [Contributing](#contributing)  
- [License](#license)  

---

## Installation  

To run this project, ensure that you have Python installed along with the required dependencies. Install them using the following command:  

```bash
pip install -r requirements.txt
bash'''
## You also need API keys for Groq and Nomic. Set them in your environment:


Copy
Edit
export GROQ_API_KEY="your_groq_api_key"
export NOMIC_API_KEY="your_nomic_api_key"
Alternatively, you can enter them manually when running the application.

## Dataset Processing
This project supports PDF documents. Once a PDF is uploaded:

The document is split into chunks for efficient retrieval.
Nomic embeddings are generated to convert text into vectors.
A FAISS vector database stores the processed text for similarity searches.
## Usage
Clone the Repository

bash
Copy
Edit
git clone https://github.com/Jyant1008/rag-chat.git
cd rag-chat
Create a Virtual Environment

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate  # Windows
Run the Application

bash
Copy
Edit
streamlit run app.py
Upload a PDF and start interacting with the chatbot!

## Models Used
Gemma2-9B-IT
LLaMA 3.1 8B Instant
Mixtral-8x7B-32768
LLaMA3-8B-8192
Each model provides a different balance of performance and efficiency.

## Embedding and Vector Search
Text Embeddings: Nomic-Embed-Text-v1.5
Vector Database: FAISS
Text Splitting: RecursiveCharacterTextSplitter
This setup ensures efficient document retrieval and fast query responses.

## Chatbot Functionality
Stores conversation history and retrieves relevant context.
Retrieves document chunks for accurate answers.
Provides step-by-step responses to user queries.
Supports clearing and restoring chat history.
## Evaluation
The chatbot is evaluated based on:

Response Relevance: Answers are compared against human-validated responses.
Retrieval Accuracy: The vector search is tested against known queries.
Performance Metrics: Latency and response times are analyzed.
## Contributing
Contributions are welcome! If you have suggestions or improvements:

Fork the repository
Create a new branch
Submit a pull request
