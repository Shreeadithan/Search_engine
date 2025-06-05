# LangChain Search Engine

This repository contains a search engine application built using LangChain, Streamlit, and various AI tools. The application provides multiple search capabilities including web search, Wikipedia, and Arxiv research paper lookups.

## Features

- Web search using DuckDuckGo
- Wikipedia article search and summarization
- Arxiv research paper search and analysis
- Interactive chat interface with streaming responses
- Agent-based architecture showing thought process
- Support for GROQ LLM integration

## Project Structure

The project consists of two main components:

1. **Streamlit Web Application (`app.py`)**
   - Interactive web interface
   - Real-time chat functionality
   - Integration with multiple search tools
   - Streaming response display
   - Session state management

2. **Jupyter Notebook (`tools_agents.ipynb`)**
   - Development and testing environment
   - Detailed implementation of search tools
   - RAG (Retrieval Augmented Generation) implementation
   - Vector store integration with FAISS
   - HuggingFace embeddings integration

## Prerequisites

- Python 3.9+
- Streamlit
- LangChain
- GROQ API access

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd <repository-name>
```

2. Install the required packages:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
Create a `.env` file in the root directory with:
```
GROQ_API_KEY=your_groq_api_key_here
```

## Usage

1. Run the Streamlit application:
```bash
streamlit run app.py
```

2. Access the web interface at `http://localhost:8501`

3. Start chatting and searching! The application supports:
   - General web searches
   - Wikipedia queries
   - Arxiv paper lookups

## Implementation Details

### Search Tools
- **Web Search**: Implemented using DuckDuckGo
- **Wikipedia**: Uses WikipediaAPIWrapper with customizable result limits
- **Arxiv**: Utilizes ArxivAPIWrapper for research paper searches

### Agent Architecture
- Uses GROQ's LLaMA 3 8b model
- Implements zero-shot agent for tool selection
- Includes StreamlitCallbackHandler for displaying agent thoughts

### User Interface
- Clean, intuitive chat interface
- Real-time response streaming
- Persistent session state
- Expandable thought process display

## Notes

- The application requires a valid GROQ API key to function
- Search results are limited to maintain performance
- The notebook version includes additional features like RAG and vector store integration

## Contributing

Feel free to submit issues, fork the repository, and create pull requests for any improvements.

## License

[Add your chosen license here] 