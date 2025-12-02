# Smart Customer Support Workflow with LangGraph

An LLM-powered customer support workflow built with LangGraph that routes user queries based on category and sentiment, and decides whether to respond automatically or escalate to a human.

## 🚀 Features
- Classifies incoming customer queries by issue type
- Performs sentiment analysis on messages
- Routes queries to:
  - automated response generator, or
  - human escalation path
- Built using LangGraph for multi-step LLM orchestration

High-level flow:
1. Ingest user query
2. Classify category (billing, technical, general, etc.)
3. Analyze sentiment (negative, neutral, positive)
4. Route:
   - If low-risk → auto-response
   - If high-risk / angry / complex → escalate

## 🛠 Tech Stack
Python, LangGraph, OpenAI API, Pydantic, Jupyter, Mermaid (for diagrams)

## 📦 Setup

```bash
git clone https://github.com/your-username/Smart-Customer-Support-Workflow-with-LangGraph.git
cd Smart-Customer-Support-Workflow-with-LangGraph
pip install -r requirements.txt
cp .env.example .env  # add your OPENAI_API_KEY
