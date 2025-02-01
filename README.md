**Overview**

**Objective:** A PDF Question Answering (QA) Chatbot that extracts information from a PDF and answers user queries.

**Core Technologies:**

**BERT:** For question answering based on the extracted context.

**FAISS:** For efficient similarity search to find relevant document chunks.

**Process:**

1.Extracts text from the PDF document.

2.Splits the text into smaller chunks.

3.Generates embeddings for each chunk using Sentence-BERT.

4.Stores embeddings in a FAISS index for fast similarity-based retrieval.

5.For each query, retrieves the most relevant chunks and uses the fine-tuned BERT model to generate an answer.

**Use Case:** Ideal for creating conversational agents that interact with large documents, such as manuals, reports, or eBooks, in a Q&A format.

**Required Libraries**

**PyMuPDF (fitz):** Used for extracting text from PDF documents.

**Sentence-Transformers:** Provides pre-trained models to generate embeddings for document chunks.

**FAISS:** Efficient similarity search library used to index and retrieve relevant chunks from document embeddings.

**Transformers (Hugging Face):** Used for loading and using pre-trained BERT models fine-tuned for Question Answering.
