# Ticker Insight

**Financial Asset Analysis AI Agent** _(Beta Version)_

> ⚠️ **Beta Release**: This is a basic proof-of-concept version for educational and experimental purposes. Not intended for actual investment decisions.

An intelligent investment research assistant built with LangGraph that analyzes stock tickers and cryptocurrency symbols, providing basic investment insights and analysis through web research and AI processing.

## 🚧 Current Status

- **Version**: 1.0.0-beta
- **Status**: Basic functionality implemented
- **Purpose**: Educational/Experimental use only
- **Investment Advice**: ❌ Not suitable for real investment decisions

## 🚀 Features

- **Multi-Asset Analysis**: Basic support for stocks and cryptocurrency symbols
- **Web-Powered Research**: Uses Tavily search API to gather publicly available information
- **AI-Driven Insights**: Leverages OpenAI's GPT models for basic analysis
- **Interactive Notebook**: Simple Jupyter notebook interface
- **Basic Reports**: Provides elementary investment potential assessments

## 📋 Prerequisites

- Python 3.13.1 or higher
- Jupyter Notebook (to run .ipynb files)
- OpenAI API key
- Tavily API key (for web search functionality)

## 🛠️ Installation

**Super Simple Setup:**

1. **Install Python 3.13.1 or higher**

   - Download from [python.org](https://www.python.org/downloads/)
   - Verify installation: `python --version`

2. **Install Jupyter**

   ```bash
   pip install jupyter
   ```

3. **Clone the repository**

   ```bash
   git clone <your-repo-url>
   cd ticker-insight
   ```

4. **Set up your API keys**

   ```bash
   cp .env.example .env
   ```

   Edit `.env` and add your API keys:

   - `OPENAI_API_KEY`: Your OpenAI API key
   - `TAVILY_API_KEY`: Your Tavily search API key

5. **Open and run the notebook**
   - Start Jupyter: `jupyter notebook`
   - Open `financial_analysis_agent.ipynb`
   - Run the cells - the notebook will install its own dependencies automatically

**That's it!** 🎉

> **Alternative**: If you use VS Code or PyCharm, they have built-in Jupyter support and can run .ipynb files directly without separate Jupyter installation.

## 🔑 Getting API Keys

### OpenAI API Key

1. Visit [OpenAI Platform](https://platform.openai.com/)
2. Sign up or log in to your account
3. Navigate to API Keys section
4. Create a new API key

### Tavily API Key

1. Visit [Tavily](https://tavily.com/)
2. Sign up for an account
3. Get your API key from the dashboard

## 🚀 Usage

1. **Start Jupyter Notebook**

   ```bash
   jupyter notebook
   ```

2. **Open the analysis notebook**

   - Navigate to `financial_analysis_agent.ipynb`
   - Run the cells step by step

3. **Test with different tickers**
   - Input any stock ticker (e.g., "AAPL", "TSLA") or cryptocurrency symbol (e.g., "BTC", "ETH")
   - The agent will research and provide comprehensive analysis

- At the end of the notebook, you can test with various stocks and crypto:

```python
# Test with Tesla stock
test_query = "Can you analyze Tesla stock for me?"
result = run_investment_research(test_query)
print("\nFinal Analysis:")
print("-" * 50)
print(result)
```

## 🤝 Acknowledgments

- Built with [LangGraph](https://github.com/langchain-ai/langgraph)
- Powered by [OpenAI](https://openai.com/)
- Web search by [Tavily](https://tavily.com/)
