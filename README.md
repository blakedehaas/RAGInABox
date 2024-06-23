# RAGInABox
A RAG agent that runs locally on your machine. Transforms your personal knowledge base into a vectorstore for contextually relevant responses. All data stays private and secure on your machine.

To create your own RAG agent, follow the steps below:
1. Add your documents to the documents folder. The documents must be .txt files. Check the process_documents directory for tools to process documents from different sources into a standard .txt file format.

2. Create a config.py file with the lines below and replace <your_api_key> with your api key for LangChain and Tavily

# config.py

LANGCHAIN_API_KEY = "<your_api_key>"
TAVILY_API_KEY = "<your_api_key>"

3. Follow the instructions in the langgraph_rag_agent_llama3_local.ipynb:
Run this command: pip install langchain-nomic
Download llama3 from ollama: Use [Ollama](https://ollama.ai/) and [llama3](https://ollama.ai/library/llama3)
Run this command after downloading: ollama pull llama3
Run all cells in the  langgraph_rag_agent_llama3_local.ipynb.

4. Modify the prompts and questions in the langgraph_rag_agent_llama3_local.ipynb to experiment with your local RAG agent and fit your specific use case.
