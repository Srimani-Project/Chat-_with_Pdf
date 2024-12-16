# Chat with PDF Using Retrieval Augmented Generation (RAG)

## Overview
The project aims to build an interactive system that allows users to chat with PDF documents. By leveraging the Retrieval-Augmented Generation (RAG) pipeline, this system enhances a model's capability to retrieve relevant information from large documents and generate meaningful, contextually aware responses. Users can ask questions or make inquiries about the content of a PDF, and the system will provide precise, extracted answers.

## Introduction 
"Chat with PDF using RAG Pipeline" is a system that allows users to interact with the content of PDF documents in a conversational manner. By leveraging Retrieval-Augmented Generation (RAG), the system retrieves relevant information from the PDF and combines it with the capabilities of a Large Language Model (LLM) to generate accurate, context-aware responses to user queries.

**The process involves**:

1. **Extracting and Chunking Text**: The PDF content is extracted, cleaned, and divided into manageable pieces for easier retrieval.

2. **Vectorization**: These chunks are converted into numerical representations (embeddings) using pre-trained models.

3. **Storage in a Vector Database**: The embeddings are stored in a database, enabling efficient similarity-based searches.

4. **Query Handling**: User queries are processed to find the most relevant chunks of text from the database.
5. **Response Generation**: The retrieved content is passed to an LLM, which generates a natural language response.
## Key Concepts:

1. **PDF Parsing and Extraction**:

 - The first step is converting the text content of a PDF into a usable format. Since PDFs can store text as well as images, the project uses libraries (e.g., PyMuPDF or pdfplumber) to extract raw text data from the document.
 2. **Retrieval-Augmented Generation (RAG)**:

- The RAG pipeline combines retrieval-based and generation-based approaches to improve response quality.
- Retrieval: In this phase, the system uses a retriever model (like a dense retriever) to search through a large document or corpus (in this case, the PDF content) and select the most relevant pieces of information.
- Augmentation: The retrieved information is then fed to a generation model (like GPT or T5), which synthesizes the extracted data and crafts a coherent and contextually relevant answer to the user's query.
3. **User Interaction (Chatbot Component)**:

- The project enables users to interact with the system through a chat interface. They can ask questions or request explanations related to specific sections of the PDF.
- The system uses the RAG model to extract relevant passages from the document and respond accordingly.

4. **Contextual and Accurate Responses**:

- The RAG pipeline ensures that the answers provided are not just generated from general knowledge but are based on the actual content within the PDF.
- This leads to more accurate and specific responses, as the system tailors its answers directly from the document's content.

## Project Features

1. **User-friendly Interface**: An intuitive interface designed to accommodate natural language queries, simplifying the interaction with PDF documents.

2. **Seamless Navigation**: The system streamlines information retrieval, reducing complexity and enhancing the overall user experience.

## Getting Started
To use this :
1. Clone the repository to your local machine.
   ```bash
   git clone https://github.com/Srimani-Project/Chat-_with_Pdf.git
   ```
2. Install dependencies.
   ```bash
   pip install -r requirements.txt
   ```
3. Run it
4. Open your browser and navigate to `http://localhost:8000` to access the user interface.
