---
title: TradingAgents: A Multi-Agent LLM Framework for Financial Trading
date: 2025-07-28
external_link: https://github.com/LuoYingyi/TradingAgents
tags:
  - Multi-Agent
  - LLM
  - Finance
  - Trading
  - LangGraph
  - Ollama
---

**TradingAgents** is a multi-agent trading framework that mirrors a real-world research & execution desk. It decomposes the workflow into specialized LLM agents—**fundamental/news/sentiment/technical analysts**, **bull/bear reviewers**, **trader**, and **risk/portfolio manager**—and coordinates them to produce end-to-end trade decisions. The system is built on **LangGraph**, supports **Finnhub** market data, and can run with either cloud LLMs or **local models via Ollama**.

<!--more-->

## Key Features
- **Role-based multi-agent collaboration:** analysts generate evidence, bull/bear reviewers debate, the trader synthesizes a plan, and risk/PM checks execution for a full decision chain.  
- **Ready-to-use CLI & Python API:** run an end-to-end session from the command line or call `TradingAgentsGraph().propagate()` in code.  
- **Configurable model stack:** mix “slow-think” and “fast-think” LLMs; tweak depth, debate rounds, and tools in `default_config.py`.  
- **Data & tools:** integrates Finnhub and supports online/offline modes for experimentation and backtesting workflows.

## What’s Innovative
- **Local LLM & privacy-friendly mode:** Ollama integration to run Qwen/Llama 3/DeepSeek locally; local embeddings to reduce cost and protect data—plus orchestration fallbacks for models without function-calling.  
- **Process transparency:** the CLI surfaces each agent’s intermediate reasoning and the final decision—great for teaching, demos, and reproducible research.  
- **From research to practice:** a clean, extensible LangGraph design that lets you test on real tickers and time windows with minimal setup.

## Getting Started
- **Install:** `pip install -r requirements.txt`  
- **Keys:** set `FINNHUB_API_KEY` (and `OPENAI_API_KEY` if using cloud LLMs)  
- **CLI:** `python -m cli.main` to choose ticker, period, and models  
- **Python:** 
  ```python
  from tradingagents.graph.trading_graph import TradingAgentsGraph
  ta = TradingAgentsGraph()
  result = ta.propagate("NVDA", "2024-05-10")
