# Assignment 2 – Chat Client

## Overview

This notebook implements a modular AI chat client called **Atlas – AI Systems Architect**.

The system demonstrates:
- Guardrails (content filtering)
- Intent classification
- Tool usage (calculator and weather)
- Retrieval-Augmented Generation (semantic search with ChromaDB)
- Multi-turn conversation support

## Services Provided

### 1. Guardrails
Blocks restricted topics before processing.

### 2. Intent Classification
Routes user queries to:
- Weather tool
- Calculator tool
- Semantic retrieval
- General LLM response

### 3. Tools

#### Weather Tool
Mock weather response using regex-based city extraction.

#### Calculator Tool
Evaluates mathematical expressions safely.

#### Semantic Search
Uses ChromaDB to retrieve relevant documents before generating responses.

## Design Decisions

- Modular architecture for clean routing.
- Separation of tools from response generation.
- Explicit routing instead of automatic tool calling.
- No additional libraries beyond course setup.
- Stateless function design for grader compatibility.

## Notes

Gradio UI was removed to comply with course environment restrictions.