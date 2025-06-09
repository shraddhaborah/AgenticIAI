AI Agentic Financial Analyst

A smart, multi-agent toolkit for financial analysis and web research—powered by Groq’s lightning-fast LLM and the versatile Phi framework.

Features

Web Search Agent: Instantly finds and summarizes information from across the web using DuckDuckGo.
Financial Analysis Agent: Tracks stock prices, analyst recommendations, company fundamentals, and the latest financial news—all in one place.
Teamwork: Agents collaborate to give you comprehensive, easy-to-understand insights.
Playground: Jump right in with an interactive web interface for chatting with your agents.

Tech Stack

AI Framework: Phi
AI Model: Groq (Llama-3-70B)
Data Sources: Yahoo Finance, DuckDuckGo
Web Interface: FastAPI
Environment: Python 3.10+ (Conda or venv)

Quick Start

Clone the repo and move into your project folder:
git clone [your-repo-url]
cd AgenticAI

Set up your environment:
conda create -n myenv python=3.10
conda activate myenv

Install dependencies:
pip install -U phidata openai duckduckgo-search yfinance fastapi sqlalchemy python-multipart python-dotenv

Configuration

Get your API keys:

Groq API Key: https://console.groq.com/keys

OpenAI API Key: https://platform.openai.com/api-keys

Phi API Key: https://phidata.com (optional)

Create a .env file in your project root:
OPENAI_API_KEY=your_openai_key
GROQ_API_KEY=your_groq_key
PHI_API_KEY=your_phi_key

How to Use

Command Line

Run your analysis directly from the terminal:
from playground import multi_ai_agent

multi_ai_agent.print_response("Tell me about NVDA stock performance", stream=True)

Web Playground

Start the interactive web interface:
python playground.py

Visit http://localhost:7777 in your browser to chat with your agents.

Example Queries

"Compare NVDA and AMD stock fundamentals"

"What’s the latest news on the semiconductor industry?"

"Show me analyst ratings for Microsoft"

Security Tips

Never commit your API keys to version control.

If you accidentally share a key, revoke it immediately.

Use environment variables for all sensitive information.

Troubleshooting

Module not found? Double-check your environment activation and installed packages.

Rate limited? Check your Groq API quota at https://console.groq.com/usage.

Authentication errors? Make sure your .env file is set up correctly.

License

MIT License

