# Research Paper Answer Bot

## Project Overview
This project develops an intelligent chatbot, the "Research Paper Answer Bot," designed to answer questions on popular Generative AI and LLM topics based on seminal research papers. Inspired by platforms like ArXiv, this system aims to revolutionize AI learning and development by providing a sophisticated RAG (Retrieval Augmented Generation) system. The core idea is to index research papers into a vector database, retrieve relevant contextual documents, and generate accurate responses. This project goes beyond a basic RAG system by exploring various advanced approaches and methodologies in each component.





## Features
+ Custom Dataset Support: While sample data is provided, the system supports loading and indexing user-provided PDF documents into a vector database.

+ Experimentation with Embedding Models: The project allows for experimentation with different embedding models, including open-source options from HuggingFace and commercial ones like OpenAI's models.
+ Diverse Retrieval Strategies: The RAG system incorporates various retrieval strategies, from simple cosine similarity to advanced hybrid search and re-rankers, to optimize context retrieval.
+ Robust RAG Pipeline: A comprehensive RAG pipeline connects the vector database to a Language Model (LLM) for generating responses.
+ Source Attribution: For transparency and verifiability, the system provides the top 3 source documents used to generate each response.
+ Multi-User Conversational RAG System: The bot is enhanced to support multi-user conversations, allowing for a more interactive and personalized experience.
+ Interactive Web Application: A Streamlit or Chainlit application provides a user-friendly interface for interacting with the RAG system.
+ Agentic Corrective RAG with Web Search: The system is further enhanced with web search capabilities using Agentic Corrective RAG patterns, allowing it to dynamically fetch information from the web when necessary, improving the accuracy and comprehensiveness of answers.

## Project Structure
```bash
├── app.py                      # Streamlit/Chainlit web application for interaction
├── scripts/
│   └── index_documents.py      # Script for loading and indexing documents into vector DB
├── research_paper_answer_bot/
│   ├── core/
│   │   ├── embeddings.py       # Module for different embedding models
│   │   ├── retrieval.py        # Module for various retrieval strategies (cosine, hybrid, rerankers)
│   │   └── rag_pipeline.py     # Core RAG pipeline logic
│   ├── agents/
│   │   └── web_search_agent.py # Agent for web search using Agentic Corrective RAG
│   └── multi_user/
│       └── conversation_manager.py # Manages multi-user conversational context
├── requirements.txt            # Python dependencies
├── README.md                   # Project README
└── .env                        # Environment variables (for API keys)
```

## Milestones Achieved
The project successfully achieved all compulsory and stretch goals:

+ Load and Index RAG documents: Implemented functionality to load and index documents into a vector database.

+ Experiment with Embeddings and build a Vector Database: Explored and integrated various open-source and commercial embedding models.

+ Experiment with various Retrieval strategies and finalize your retriever: Conducted experiments with different retrieval strategies, including hybrid search and re-rankers.

+ Build basic RAG system with answer sources: Developed a functional RAG pipeline that provides source attribution for generated responses.

+ Build enhanced RAG system or application based on stretch goals:
+ Advanced Option 1: Multi-user Conversational RAG System: The system is designed to handle multiple users and maintain conversational context.
+ Advanced Option 2: Streamlit/Chainlit App: A user-friendly web interface has been built for interaction.
+ Advanced Option 3: Agentic Corrective RAG with Web Search: Integrated web search capabilities to enhance answer accuracy and breadth.
