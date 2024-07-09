# PDF Chat with Google Generative AI

This project is a Streamlit application that enables users to chat with PDF documents using Google's Generative AI. It allows users to upload PDFs and ask questions about their content, with the AI providing detailed answers based on the information in the documents.

## Project Overview

The application combines several key technologies and techniques:

1. PDF Processing: Extracts text from uploaded PDF files.
2. Text Chunking: Splits large texts into manageable chunks for efficient processing.
3. Embeddings: Uses Google Generative AI to create embeddings of the text chunks.
4. Vector Store: Implements FAISS for similarity search on the embeddings.
5. Question-Answering: Utilizes Google's Generative AI to answer user queries based on the PDF content.

## Key Implementations

1. PDF Text Extraction
   - Uses PyPDF2 to read and extract text from uploaded PDF files.

2. Text Chunking
   - Implements RecursiveCharacterTextSplitter from LangChain to divide large texts into smaller, overlapping chunks.

3. Embedding Generation
   - Utilizes GoogleGenerativeAIEmbeddings to create vector representations of text chunks.

4. Vector Store Creation
   - Employs FAISS to create a searchable index of the text embeddings.

5. Conversational Chain
   - Implements a question-answering chain using ChatGoogleGenerativeAI.
   - Uses a custom prompt template to guide the AI in providing detailed answers.

6. User Interface
   - Builds an interactive interface using Streamlit, allowing users to upload PDFs and ask questions.

7. Answer Generation
   - Combines similarity search results with the conversational chain to generate relevant answers to user queries.

This project demonstrates the integration of advanced NLP techniques with a user-friendly interface, enabling efficient information retrieval from PDF documents through natural language queries.
