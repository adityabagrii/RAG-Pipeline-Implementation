# RAG Pipeline
## What is RAG?
RAG stands for Retrieval-Augmented Generation, an AI framework that combines information retrieval systems with large language models (LLMs). RAG improves the quality of LLM responses by allowing them to access information outside of their training data. 
### How it works
- RAG uses search algorithms to query external data, such as databases, knowledge bases, and web pages 
- The retrieved information is pre-processed 
- The pre-processed information is integrated into the pre-trained LLM 
- The LLM generates a response using the retrieved information 
### Benefits
- RAG can produce more relevant, accurate, and up-to-date text 
- RAG is a cost-effective way to improve LLM output 
- RAG can produce highly specific outputs without extensive fine-tuning or training 

This repositry contains an implementation of a RAG pipeline using HuggingFace Embeddings, MistralAI and LangChain to work on the Data stored as PDFs in the Data Folder. It reads all the data creates indexing and vector embeddings using HuggingFaces "sentence-transformers/all-mpnet-base-v2" model and then creates a retriever which gathers all the relevant material while prompting MistralAI about the users query to produce better and relevant results to the data provided.

### Example
I have used the B.Tech Regulations of my college to run tests on the pipeline.