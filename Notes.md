# Notes

## Embeddings and RAG (2026-11-16)
- Chunking: I split a big document into small pieces called chunks. This is a choice I make, and my project tests 4 ways of doing it.
- Embedding: an embedding is a list of numbers that represents the meaning of one chunk. Similar meanings get similar numbers.
- Storing: I store every chunk's embedding in a vector database (Chroma).
- Retrieval: when a user asks a question, I convert the question into numbers with the same embedding model. The database returns the chunks whose numbers are closest.
- Generation: I give those chunks and the question to the LLM, and it writes the answer from them.
- Why not exact word search: people ask the same thing in different words. "How do I install it?" and "Steps to set up the library" share almost no words, but embeddings match them by meaning.