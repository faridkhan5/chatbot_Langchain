# Intro to LangChain

## 1. LangChain Tracing
  * Configures environment variables for OpenAI and LangChain tracing.
  * Defines a prompt template for user queries.
  * Sets up a chain combining a ChatOpenAI model and an output parser to process and display responses.

## 2. Essay and Poem Generation with LangChain
  * Sets up a FastAPI server with routes to generate essays and poems using LangChain and LLMs (ChatOpenAI and OllamaLLM).
  * Defines prompts and connects them to endpoints (/essay and /poem), making them accessible for API requests.

## 3. Simple RAG Pipeline
  * Load data from data source.
  * Split data into chunks.
  * Convert chunked data into vector embeddings and store them in FAISS vector database.