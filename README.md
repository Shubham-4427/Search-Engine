# Search Engine

> An AI-powered search assistant that answers user queries using real-time web search, Wikipedia knowledge retrieval, and Arxiv research paper search through a LangChain agent.

---

## Project Overview

**Search Engine** is an AI-powered search chatbot designed to provide intelligent and tool-assisted answers to user queries.

Instead of relying only on the language model's internal knowledge, the system uses external search tools to retrieve relevant information from multiple sources.

Users can:

* Ask general questions
* Search the web using DuckDuckGo
* Retrieve factual information from Wikipedia
* Explore academic and research-based content from Arxiv
* Interact through a clean Streamlit chat interface
* Use Groq's Llama 3 model for fast AI-generated responses

The system combines Large Language Models with external search tools to create a lightweight AI search engine experience.

---

## System Architecture

```text
User Query
    │
    ▼
Streamlit Chat Interface
    │
    ▼
LangChain Agent
    │
    ├── DuckDuckGo Search Tool
    │
    ├── Wikipedia Search Tool
    │
    └── Arxiv Research Tool
    │
    ▼
Groq Llama 3 Model
    │
    ▼
Final AI Response
```

The architecture follows an agent-based design where the LangChain agent decides which tool to use based on the user's query.

---

## Technology Stack

| Layer | Technology |
| ------------------- | ---------------- |
| Interface | Streamlit |
| Core Language | Python |
| LLM Framework | LangChain |
| LLM Provider | Groq |
| Model | Llama3-8b-8192 |
| Web Search | DuckDuckGo Search |
| Knowledge Retrieval | Wikipedia API |
| Research Retrieval | Arxiv API |
| Environment Management | python-dotenv |

---

## Project Structure

```text
Search-Engine/
│
├── app.py                 # Main Streamlit application
├── requirements.txt       # Project dependencies
├── tools_agents.ipynb     # Notebook for tool and agent experimentation
├── README.md              # Project documentation
└── LICENSE                # License file
```

---

## Core Features

* AI-powered search chatbot
* Real-time web search using DuckDuckGo
* Wikipedia-based factual information retrieval
* Arxiv-based academic paper search
* LangChain agent with tool-calling capability
* Groq Llama 3 integration
* Streamlit-based interactive chat UI
* Session-based chat history
* Streaming response support

---

## How It Works

1. The user enters a query in the Streamlit chat interface.
2. The query is passed to a LangChain agent.
3. The agent decides whether to use:
   * DuckDuckGo for web search
   * Wikipedia for factual knowledge
   * Arxiv for academic research
4. The selected tool retrieves relevant information.
5. Groq's Llama 3 model generates the final response.
6. The answer is displayed in the chat interface.

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Shubham-4427/Search-Engine.git
cd Search-Engine
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

---

## Usage

Run the Streamlit app:

```bash
streamlit run app.py
```

Then open the local Streamlit URL in your browser.

Enter your Groq API key in the sidebar and start asking questions.

---

## Example Questions

```text
What is machine learning?
```

```text
Search latest AI news
```

```text
Find research papers on transformers
```

```text
Who is Alan Turing?
```

```text
Explain quantum computing
```

---

## Production-Grade Design Principles

* Agent-based architecture for flexible tool usage
* Separation of UI, model, and search tools
* External knowledge retrieval for improved responses
* Lightweight and interactive Streamlit interface
* Modular tool integration using LangChain
* API-key based secure model access

---

## Future Enhancements

* Add support for document-based search
* Add PDF upload and summarization
* Add YouTube video summarization
* Add source citations in final answers
* Add vector database support using FAISS or ChromaDB
* Add conversation memory
* Add user authentication
* Deploy on Streamlit Cloud, Render, or Hugging Face Spaces
* Improve UI with better chat styling
* Add support for multiple LLM providers

---

## Author

**Shubham Kumar**  
AI Developer | Machine Learning Engineer | Creative Technologist

---

⭐ If you find this project useful, consider giving it a star on GitHub.
