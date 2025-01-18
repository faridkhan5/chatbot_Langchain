# Intro to LangChain

## 1. LangChain Tracing
  * Configures environment variables for OpenAI and LangChain tracing.
  * Defines a prompt template for user queries.
  * Sets up a chain combining a ChatOpenAI model and an output parser to process and display responses.

## 2. Essay and Poem Generation with LangChain
  * Sets up a FastAPI server with routes to generate essays and poems using LangChain and LLMs (ChatOpenAI and OllamaLLM).
  * Defines prompts and connects them to endpoints (/essay and /poem), making them accessible for API requests.

## 3. Simple RAG Pipeline
  * Loads data from data source.
  * Splits data into chunks.
  * Converts chunked data into vector embeddings and store them in FAISS vector store.

## 4. Retrieval Chain
  * Loads, splits, coverts documents and stores their vector embbedings in a FAISS vector store.
  * Initializes an Ollama LLM (llama2) and a ChatPromptTemplate for context-based question answering.
  * Creates a document chain to combine retrieved documents with the LLM and prompt.
  * Set up a retriever to fetch relevant documents from a vector store (db).
  * Combines the retriever and document chain to create a retrieval chain.
  * Executes the retrieval chain to process the query and generate a response.