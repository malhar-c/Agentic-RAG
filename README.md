# Agentic RAG - Proof of Concept

## Overview

This is a **Proof of Concept (POC)** for a sophisticated RAG (Retrieval-Augmented Generation) Agent that forms part of a larger ambitious project: building a **J.A.R.V.I.S.-like personal assistant**.

## Project Vision

The ultimate goal is to create an intelligent personal assistant that combines:

- **Static Knowledge Layer**: A fine-tuned small multimodal LLM (~7B parameters) trained with static personal information, values, and ethics to run entirely on local machines
- **Dynamic Knowledge Layer**: Sophisticated RAG agents (like this POC) that handle evolving personal and private information that changes over time
- **Privacy-First Architecture**: Ensuring all personal data remains local and secure

## ⚠️ Project Sensitivity Notice

This is an **extremely sensitive project** dealing with personal AI systems and private information processing. Due to the nature of this work involving:

- Personal data handling architectures
- Privacy-preserving AI systems
- Local LLM fine-tuning methodologies
- Advanced RAG implementations for personal use

**Only Proof of Concept implementations will be made publicly available.** The core system designs, training methodologies, and production implementations remain private to ensure responsible development and deployment of personal AI technologies.

## Current POC Features

This RAG agent demonstrates:

- Web scraping and document ingestion using FireCrawl
- Document chunking and embedding with local models
- Vector storage using ChromaDB
- Retrieval grading and relevance assessment
- Local LLM integration (Llama3) for privacy

## Setup

### Prerequisites

- Python 3.8+
- Local Ollama installation with Llama3 model
- API keys for external services

### Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -U langchain-nomic langchain_community tiktoken langchainhub chromadb langchain langgraph tavily-python gpt4all firecrawl-py
   ```
3. Get your API keys:
   - LangChain: https://smith.langchain.com/
   - FireCrawl: https://firecrawl.dev/
4. Update the API keys in the notebook (replace placeholder values)
5. Ensure Ollama is running locally with Llama3 model
6. Run the notebook

### Configuration

Replace the placeholder API keys in the notebook:

```python
os.environ['LANGCHAIN_API_KEY'] = 'your_langchain_api_key_here'
os.environ['FIRECRAWL_API_KEY'] = 'your_firecrawl_api_key_here'
```

## Architecture Notes

This POC focuses on the **dynamic knowledge component** of the larger system, showcasing how private information can be processed and retrieved while maintaining local execution for sensitive operations.

## Future Development

- Integration with fine-tuned personal LLM
- Enhanced multimodal capabilities
- Improved privacy and security measures
- Advanced agent orchestration
- Real-time learning and adaptation

## Disclaimer

This repository contains only educational and demonstration components. The complete system architecture and implementation details are not disclosed due to the sensitive nature of personal AI assistant development.

---

\_This project represents a step toward truly personal AI assistants that respect privacy while providing powerful, context-aware assistance.
