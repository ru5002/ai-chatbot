# AI Restaurant Menu Chatbot

An intelligent chatbot built with LlamaIndex, Groq LLM, and Gradio that helps customers
explore a restaurant menu through natural language queries. The chatbot uses Retrieval-
Augmented Generation (RAG) to provide accurate responses about menu items, prices,
ingredients, dietary preferences, and spice levels.

## Features

- Natural language queries for menu exploration
- Smart filtering by price range, dietary restrictions, and spice level
- Detailed ingredient information for all menu items
- Price comparisons and recommendations
- Interactive web interface powered by Gradio

## Prerequisites

- Python 3.8 or higher
- Groq API Key from https://console.groq.com
- Git for version control

## Installation

Clone the repository:
```
git clone https://github.com/ru5002/ai-chatbot.git
cd ai-chatbot
```

Create and activate virtual environment:

Windows PowerShell:
```
python -m venv venv
.\venv\Scripts\Activate.ps1
```

Windows Command Prompt:
```
python -m venv venv
.\venv\Scripts\activate.bat
```

Linux/Mac/Git Bash:
```
python -m venv venv
source venv/bin/activate
```

Install dependencies:
```
pip install -r requirements.txt
```

## Configuration

Create a .env file from the example:
```
cp .env.example .env
```

Add your Groq API key to .env:
```
GROQ_API_KEY=your_actual_groq_api_key_here
```

Note: Never commit your .env file to Git.

## How to Run

Launch Jupyter Notebook:
```
jupyter notebook
```

Open chatbot.ipynb and run all cells sequentially.

## Technical Details

Architecture:
- LLM: Groq Llama-3.1-8b-instant
- Embeddings: HuggingFace sentence-transformers/all-MiniLM-L6-v2
- Vector Store: LlamaIndex VectorStoreIndex
- UI: Gradio chat interface

---

**Enjoy chatting with the AI Restaurant Assistant! 🍽️**
