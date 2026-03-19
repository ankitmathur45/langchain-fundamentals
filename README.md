# 🦜 LangChain Fundamentals

A structured, hands-on introduction to LangChain built on a local 
Llama 3.2 model via Ollama. No API costs. No internet required.

## What This Covers
Three core LangChain concepts, one notebook each, built progressively:

### 01 — Prompt Templates
- OllamaLLM basics — provider abstraction
- PromptTemplate for reusable dynamic prompts
- ChatPromptTemplate for system + human message structure
- Persona comparison demonstrating system prompt power

### 02 — Chains
- The problem with manual multi-step LLM calls
- LCEL pipe operator `|` connecting prompt → LLM → parser
- RunnablePassthrough.assign for multi-step pipelines
- Full product naming pipeline across multiple inputs

### 03 — Memory
- Stateless problem demonstration
- Manual memory via message history list
- MessagesPlaceholder for injecting history into chains
- ConversationManager — reusable pattern for any chat app

## Git Workflow
This repo was built using a real team Git workflow:
- Each concept lives on its own feature branch
- Every branch merged via Pull Request
- Conventional commit messages throughout

## Setup
```bash
git clone git@github.com:ankitmathur45/langchain-fundamentals.git
cd langchain-fundamentals
uv venv .venv --python 3.12
.venv\Scripts\activate
uv pip install -r requirements.txt

# Install and run Ollama
# https://ollama.com/download
ollama pull llama3.2
```

Open notebooks in order — 01, 02, 03. Select Python (langchain-fundamentals) kernel.

## Tech Stack
- Python 3.12
- LangChain + LangChain Core
- LangChain Ollama
- Llama 3.2 (local via Ollama)