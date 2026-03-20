# 🚀 AI Trading System

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)]()
[![FastAPI](https://img.shields.io/badge/API-FastAPI-009688.svg)]()
[![LangGraph](https://img.shields.io/badge/Workflow-LangGraph-purple.svg)]()
[![Status](https://img.shields.io/badge/Status-Active%20Development-orange.svg)]()

> **A multi-agent AI system for financial analysis, signal generation, and backtesting**
>
> Designed for **researchers**, **students**, and **recruiters** who want to explore practical AI system design, hybrid decision workflows, and applied financial intelligence.

---

## 📌 Overview

The **AI Trading System** is an open-source project that combines **multi-agent reasoning**, **local signal generation**, and **hybrid AI workflows** to analyze financial assets from multiple perspectives.

Instead of depending on a single model or fixed rule, the system coordinates multiple specialized components such as:

- 📈 **Technical Analysis Agent**
- 📰 **Sentiment Analysis Agent**
- ⚠️ **Risk Management Agent**
- 🧠 **Portfolio Decision Agent**

The project supports:

- **Local signal generation** for fast, low-cost, deterministic analysis
- **LLM-powered analysis** for contextual and language-based reasoning
- **Hybrid decision workflows** with intelligent escalation logic

> **Note:** This project is built for **education, experimentation, and research**. It is **not intended for live trading or financial advice**.

---

## ✨ Why This Project Stands Out

### 🔬 For Researchers
- Explore **graph-based agentic workflows**
- Study **hybrid decision systems** that combine deterministic logic with LLM reasoning
- Experiment with **signal validation**, **conflict detection**, and **market regime detection**
- Compare **local vs LLM-based analysis** for speed, cost, and reliability

### 💼 For Recruiters
This project highlights:
- Strong **system design**
- Modular **Python backend development**
- **FastAPI** API engineering
- Agent orchestration using **LangGraph**
- Clean project organization and scalable architecture
- Testing, migration, extensibility, and separation of concerns

### 🎓 For Students
- Learn how AI can be applied in finance through a practical system
- Understand how multiple modules collaborate in a real project
- Study API development, CLI design, testing workflows, and agent-based architecture

---

## 🤖 Why Use Agents in Trading?

Traditional trading systems often rely on one model, one strategy, or one decision pipeline. In contrast, an **agent-based trading system** breaks the problem into specialized responsibilities.

### Benefits of Agents in Trading
- **Specialization:** Each agent focuses on one task such as technical analysis, sentiment interpretation, or risk control
- **Explainability:** Individual agent outputs make the final decision easier to understand
- **Modularity:** New agents can be added without redesigning the whole system
- **Robustness:** Conflicting views from multiple agents can improve decision quality
- **Scalability:** Agents can be extended for new data sources, strategies, and asset classes

### Agent Roles in This Project
- 📈 **Technical Analysis Agent**  
  Studies price action, moving averages, momentum indicators, and chart-based signals

- 📰 **Sentiment Analysis Agent**  
  Interprets financial news, market sentiment, and text-driven signals

- ⚠️ **Risk Management Agent**  
  Evaluates exposure, uncertainty, volatility, and trade safety

- 🧠 **Portfolio Decision Agent**  
  Combines inputs from other agents and produces the final trading signal

This design makes the system more aligned with how real-world financial decision processes are often structured: multiple viewpoints, layered validation, and controlled execution logic.

---

## 🛠️ Tech Stack

### Core Technologies
- **Python 3.10+** – Primary development language
- **FastAPI** – High-performance REST API framework
- **LangGraph** – Graph-based orchestration for multi-agent workflows
- **uv** – Dependency and environment management
- **pytest** – Testing and validation

### AI / Analysis Layer
- **LLM Providers:** OpenAI, Anthropic, Groq, Google, OpenRouter
- **Local Signal Engine:** Deterministic rule-based and weighted signal generation
- **Technical Analysis Components:** Indicator scoring, market regime detection, validation, and consensus logic

### Data & Infrastructure
- **yfinance / Alpha Vantage / Finnhub / MarketAux** – Market and sentiment data providers
- **Redis (optional)** – Caching for performance optimization
- **CLI + FastAPI API** – Dual interface for developers and end users

### Engineering Highlights
- Multi-agent orchestration
- RESTful API design
- CLI tooling
- Backtesting workflow
- Migration framework
- Organized testing architecture

---

## 🌟 Features

- 🤖 **Multi-Agent Analysis**  
  Specialized AI agents analyze markets from technical, sentiment, risk, and portfolio perspectives.

- ⚡ **Local Signal Generation Framework**  
  Generate trading signals without relying on LLM calls, reducing latency and cost.

- 🔁 **Hybrid Signal Generation**  
  Seamlessly combines local logic and LLM-based intelligence with escalation mechanisms.

- 🕸️ **Graph-Based Workflow**  
  Uses **LangGraph** to manage agent communication and decision flow.

- 🔌 **Extensible Provider Network**  
  Supports multiple market data and LLM providers.

- 🌐 **REST API**  
  Built with **FastAPI** for easy integration with external systems.

- 🧪 **Backtesting Support**  
  Includes tools to evaluate trading strategies on historical data.

- 🧱 **Migration Framework**  
  Enables gradual migration from LLM-only workflows to hybrid/local approaches.

---

## 🧠 Local Signal Generation Framework

The **Local Signal Generation Framework** enables fast and reliable signal creation without external LLM calls.

### ✅ Benefits
- **Performance:** Signal generation latency reduced from seconds to milliseconds
- **Cost Efficiency:** Minimizes LLM API usage
- **Reliability:** Less dependent on external AI services

### 🧩 Core Components
1. **Market Regime Detector** – Identifies trending, ranging, or volatile markets  
2. **Indicator Scorer** – Scores multiple technical indicators  
3. **Consensus Signal Combiner** – Aggregates weighted signals  
4. **Hierarchical Decision Tree** – Produces final signal decisions  
5. **Signal Validator** – Validates outputs using market context  
6. **Conflict Detector** – Detects contradictions across signal sources  
7. **LLM Escalation Logic** – Escalates only when deeper reasoning is needed  

### 📍 Supported Signal Types
- 🟢 **BUY**
- 🔴 **SELL**
- 🟡 **HOLD**

Each signal includes:
- Signal strength (`WEAK`, `MODERATE`, `STRONG`, `VERY_STRONG`)
- Confidence score (`0.0` to `1.0`)
- Market regime
- Human-readable reasoning
- Contributing indicators and weights

---

## 🏗️ Architecture

For a detailed explanation of system design, workflow, and components, see the [**Architecture Document**](docs/ARCHITECTURE.md).

### High-Level Workflow
1. **Collect market and sentiment data**
2. **Pass information through specialized agents**
3. **Combine local and/or LLM-based reasoning**
4. **Validate signal quality**
5. **Return structured trading decision**

---

## 🚀 Getting Started

Follow these steps to run the project locally for development and testing.

### Prerequisites
- Python 3.10+
- [uv](https://github.com/astral-sh/uv)
- Active internet connection

### Installation

#### 1. Clone the repository
```sh
git clone https://github.com/your-username/ai-trading-system.git
cd ai-trading-system
