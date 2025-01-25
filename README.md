# Question-Answering System Powered by LangChain and LLM

This project implements a fully functional **Question-Answering (QA) system** that leverages **LangChain** and a **Large Language Model (LLM)** to process PDF documents and answer user queries effectively. The system is designed to efficiently handle document processing, semantic search, and answer generation using state-of-the-art technologies. It includes components such as document loaders, chunk splitting, embeddings, vector database storage, a retriever, and an LLM as a generator. **Gradio** is used for building an intuitive web interface for user interaction.

## Features

- **Document Loader**: Loads PDF documents and prepares them for further processing.
- **Chunk Splitting**: Divides the documents into smaller, manageable chunks to facilitate efficient processing and retrieval.
- **Embeddings**: Converts document chunks into embeddings, capturing their semantic meaning for fast and accurate querying.
- **Vector Database**: Stores the embeddings in a vector database for quick retrieval of relevant chunks.
- **Retriever**: Retrieves the most relevant document chunks based on user queries.
- **LLM as Generator**: Uses a Large Language Model (LLM) to generate accurate answers from the retrieved document chunks.
- **Gradio Interface**: A simple, interactive web interface built using Gradio, allowing users to query the system easily.

## Technologies Used

- **LangChain**: A framework for building applications with language models, which orchestrates the flow of documents, embeddings, and retrievals.
- **Large Language Model (LLM)**: Used for generating answers based on the retrieved document chunks. You can use any suitable model, such as GPT-3, GPT-4, or a fine-tuned model.
- **PDF Processing**: Libraries like `PyMuPDF` or `pdfminer` for extracting text from PDF files.
- **Embeddings**: Utilizes models like **Sentence-BERT**, **OpenAI's embeddings**, or similar models to create dense vector representations of text.
- **Vector Database**: **FAISS**, **Pinecone**, or similar for storing and retrieving high-dimensional embeddings efficiently.
- **Retriever**: A retriever component based on the vector database that performs nearest-neighbor search to find relevant chunks.
- **Gradio**: A Python library used to create user-friendly interfaces for machine learning applications.

## Installation

### 1. Clone the Repository
Clone this repository to your local machine:
```bash
git clone https://github.com/sasidhar791/QA_Bot.git
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```
### 3. Set Up Vector Database and Model Configuration
Ensure that your vector database (e.g., FAISS, Pinecone) and model configurations (e.g., OpenAI API key) are properly set up before using the system.

## Usage
### 1. Run the QA System
After setting up the repository and installing dependencies, run the Python script to start the QA system:
```bash
python QA_bot.py
```

### 2. Access the Web Interface
Once the script is running, the Gradio interface will be hosted on your local machine. Open a web browser and navigate to the following URL:
```bash
http://127.0.0.1:7860
```

### 3. Upload a PDF and Submit a Query
On the webpage, you will see an option to upload a PDF document. Upload your desired PDF file, enter your query in the input box, and click the Submit button.


### 4. View the Output
After submitting your query, the system will process the PDF and return an answer based on the content of the PDF.

## Contributing
We welcome contributions to this project! If you'd like to contribute, please feel free to fork the repository, submit issues, or create pull requests.

