# RAG-System-using-LLaMA-2-ChromaDB
This project implements a Question-Answering (QA) System that extracts knowledge from scientific papers and answers user queries using LLaMA-2 and ChromaDB. The pipeline enables document parsing, text chunking, vector embedding, and context-based response generation without relying on pre-trained QA pairs.

# Features:

 PDF Parsing: Uses PyPDFLoader to read and split the PDF into manageable text chunks.

 Text Chunking: Employs RecursiveCharacterTextSplitter for optimal chunk size and overlap to maintain context.

 Vector Database: Stores text embeddings using ChromaDB for efficient retrieval.

 Embedding Model: Utilizes all-miniLM-L6-v2 from sentence-transformers for lightweight yet effective text embeddings.

 LLM Integration: Loads the LLaMA-2-7b-chat model for generating context-aware responses.

 Contextual Retrieval: Implements a retriever to fetch the top relevant chunks based on user queries.

 Prompt Engineering: Uses a custom prompt template to guide the LLM's responses.

# Workflow:

  PDF Loading → Extracts and splits PDF content.

  Text Embedding → Converts text chunks into vector representations.

  Vector Storage → Saves embeddings in ChromaDB for fast retrieval.

  Query Processing → Retrieves relevant chunks based on the query.

  Response Generation → Feeds context to LLaMA-2 and generates answers.

# Tech Stack:

Python

 PyTorch

 Transformers (HuggingFace)

 Langchain

 ChromaDB

 LLaMA-2 7B

 Sentence Transformers
