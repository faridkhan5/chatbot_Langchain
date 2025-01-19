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

## 5. RAG Pipeline with Multiple Tools
  * Creates specialized tools for retrieving information from LangSmith (retriever_tool), Wikipedia (wiki), and ArXiv (arxiv), each with tailored constraints.
  * Combines a ChatOpenAI model with the tools using a pre-defined prompt from Hugging Face, enabling the agent to reason and utilize the tools effectively.
  * Constructs an agent using create_openai_tools_agent, allowing dynamic interaction between the LLM and tools for answering queries.
  * Executes the query, with the AgentExecutor deciding which tools to use and synthesizing the final response.