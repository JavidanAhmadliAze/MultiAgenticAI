# Multi-Agent Research Workflow with AI

This project implements a **multi-agent AI system** for automating research workflows using the **Groq LLM** and the **LangGraph** framework. It demonstrates how a set of AI agents can collaborate to perform complex research tasks, including collecting papers, ranking them, identifying gaps, and refining research focus.

---

## Features

- **Supervisor Agent:** Manages the workflow, decides which agent should act next based on current state.
- **Scraper Agent:** Collects recent research papers from arXiv for a given task.
- **Ranker Agent:** Ranks scraped papers by relevance to the research topic.
- **Gap Finder Agent:** Identifies gaps or underexplored areas in the research.
- **Feedback Agent:** Refines research focus and generates actionable insights.
- **Workflow Engine:** Uses `LangGraph` to orchestrate agent interactions and maintain state across iterations.
- **LLM-Driven Decisions:** Groq LLM is used to make decisions and provide summaries.

---

## Workflow

1. **Supervisor** decides the next agent based on task progress.
2. **Scraper** collects research papers.
3. **Ranker** evaluates and ranks collected papers.
4. **Gap Finder** detects missing areas or open questions.
5. **Feedback** generates refined research directions.
6. **Supervisor** iterates until the task is complete.

---

## Tech Stack

- Python 3.x
- [Groq LLM](https://www.groq.com/)  
- [LangGraph](https://github.com/langgraph/langgraph) for workflow orchestration  
- LangChain `AIMessage` & `HumanMessage` for agent communication  
- [arXiv API](https://arxiv.org/help/api/index) for research paper collection  

---

## Installation

```bash
git clone https://github.com/JavidanAhmadliAze/MultiAgenticAI.git
cd MultiAgenticAI
uv add -r requirements.txt


