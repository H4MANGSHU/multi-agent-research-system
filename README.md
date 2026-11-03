# multi-agent-research-system


A multi-agent research system built to handle complex, cross-domain queries by orchestrating specialized AI agents.

## Architecture

The system uses an **Orchestrator Pattern** where a primary controller agent evaluates the user's prompt and dynamically routes tasks to domain-specific specialist agents:
1. **Financial Analyst**: Handles SEC filings, stock pricing, earnings reports, and macroeconomic indicators.
2. **Scientist**: Focuses on biomedical papers, clinical trials, and FDA data tracking.
3. **Journalist**: Performs real-time web research and news gathering.

---

## Project Structure

```text
multi-agent-research-system/
├── src/
│   ├── agents/
│   │   ├── orchestrator.py (or route.ts)
│   │   ├── financialAgent.py
│   │   ├── scientistAgent.py
│   │   └── journalistAgent.py
│   ├── tools/
│   │   ├── searchTools.py
│   │   └── apiConnectors.py
│   └── main.py
├── .env.example
├── requirements.txt
└── README.md
