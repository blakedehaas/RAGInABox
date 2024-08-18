# RAGInABox
A fully contained RAG agent that runs locally on your machine. Transforms your personal knowledge base into a vectorstore for contextually relevant responses. Also has the capability to search the internet for relevant documents when none of your documents are relevant. All data stays private and secure on your machine. 

To create your own RAG agent, follow the steps below:

1. Download CUDA Toolkit for your operating system to use the GPU:

https://developer.nvidia.com/cuda-downloads

2. Download ollama from their website for your operating system:

https://ollama.com/

3.  In your terminal, download llama3 with this command:

ollama pull llama3

4. Add your documents to the documents folder. The documents must be .txt files. Check the process_documents directory for tools to process documents from different sources into a standard .txt file format.

5. Create a config.py file with the lines below and replace <your_api_key> with your api key for LangChain and Tavily:

LANGCHAIN_API_KEY = "<your_api_key>"

TAVILY_API_KEY = "<your_api_key>"

6. In your terminal, navigate to the RAGInABox directory and run the application with this command:

python3 main.py

7. Follow the instruction in the terminal to ask the RAG agent questions.

8. Experiment with the prompts in main.py to fit the RAG agent to your specific use case.
