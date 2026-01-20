
# AI-Assisted Trader

**AI-Assisted Trader** is a human-in-the-loop intraday trading system designed to identify high-probability momentum moves before the market reacts.  
It combines **real-time news analysis**, **technical filters**, and **risk-managed execution** with AI reasoning to assist trading decisions — all while keeping the human in control.

---

## Key Features

- **News-First Scanning:** Detect potential movers from real-time news and market data before the crowd.
- **Rule-Based Filtering:** Price, float, volume, and market cap filters remove low-probability trades automatically.
- **AI-Assisted Analysis:** LangChain evaluates catalysts and provides reasoning while respecting deterministic rules.
- **Human-in-the-Loop Approval:** Trades are proposed to the user for confirmation before execution.
- **Paper Trading Execution:** Safely test the system using paper trading APIs.
- **Risk Management:** Stop-loss, partial exits, and time-based rules enforce discipline.
- **Post-Trade Review:** AI-assisted summaries analyze trade performance and highlight insights for continuous learning.

---

## Core Workflow

1. **News & Market Data Ingestion**  
   Gather breaking news, float, volume, price, and market cap.

2. **Rule-Based Filtering**  
   Apply deterministic filters to remove low-probability candidates.

3. **AI Catalyst Analysis**  
   Classify catalysts and assess their strength using LLMs.

4. **Trade Proposal & Human Approval**  
   Present trade plan (entry, stop, target, probability) for human review.

5. **Paper Trade Execution**  
   Execute approved trades while enforcing risk rules.

6. **Trade Monitoring & Exit**  
   Track momentum, partial exits, and stop-loss enforcement.

7. **Post-Market Review**  
   Summarize trade performance, learn from successes and failures.

---

## Tech Stack

- **LangChain:** AI reasoning & news analysis  
- **LangGraph:** Workflow orchestration & human-in-the-loop control  
- **Market Data:** NewsAPI, GNews, Yahoo Finance, Polygon, etc.  
- **Paper Trading:** Alpaca, Interactive Brokers, or equivalent API  
- **Backend / Scheduler:** FastAPI / cron jobs / WebSocket  
- **UI (Optional):** Web interface or Slack/Telegram bot for human approvals

---
