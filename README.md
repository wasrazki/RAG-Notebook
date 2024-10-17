# Description:

In this project, I developed a Retrieval-Augmented Generation (RAG) pipeline from scratch using Python to enable efficient and accurate information retrieval from a nutrition-related PDF document. The system processes the entire document, splits it into manageable text chunks, and allows for precise semantic search and question-answering using deep learning models.

# Key Features:

- PDF Parsing and Preprocessing: Extracted text from the PDF, clean and format the content, and generate metadata such as word, sentence, and token counts for each page.
- Sentence Splitting and Chunking
- Sentence Embedding: Leveraged Sentence-Transformers to encode the text chunks into embeddings.
- Query Retrieval and Similarity Search: Implemented semantic search using dot-product similarity to retrieve the most relevant text chunks corresponding to the user’s query .
- Generative Answering with a Large Language Models: Integrated a pre-trained language model (Google's Gemma-7B) with attention mechanisms and quantization for memory efficiency. The model generates natural-language answers based on the retrieved context.

# Implementing RAG from Scratch: How It Differs from Existing Solutions

Building RAG from scratch differs significantly from using pre-built RAG frameworks in the following ways:
- Custom Document Processing: Instead of using pre-processed datasets, I implemented the entire document ingestion and processing pipeline (text extraction, cleaning, sentence splitting, chunking), providing more control over the granularity of chunks and the metadata captured.
- Manual Retrieval Pipeline: I wrote my own retrieval system using Sentence-Transformers for encoding text chunks and dot-product similarity for ranking, whereas traditional RAG implementations rely on pre-built similarity or retrieval modules. This gave me flexibility in embedding generation and search methodology.
  
