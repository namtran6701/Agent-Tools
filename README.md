# Yahoo Finance Agent

This notebook demonstrates how to use the Yahoo Finance API to create a financial analysis agent using LangChain and OpenAI's language models. The agent can retrieve news, perform fundamental analysis, and provide insights on stocks.

## Features

- Yahoo Finance News retrieval
- Stock ticker symbol extraction
- Fundamental financial analysis
- Simple DCF valuation

## Requirements

- Python 3.7+
- Libraries: 
  - yfinance==0.2.44
  - langchain==0.3.1
  - langchain-community==0.3.1
  - langchain-openai==0.2.1
  - langchain-core==0.3.8
  - pandas==2.2.3
  - pydantic==2.9.1

## Setup

1. Clone this repository
2. Install the required libraries:
   ```
   pip install -r requirements.txt
   ```
3. Set up your OpenAI API key in a `.env` file

## Usage

The notebook contains two main sections:

1. **Yahoo Finance News**: Demonstrates how to retrieve recent news about a company using both an AgentExecutor and a Pydantic approach.

2. **Financial Research**: Performs a comprehensive fundamental analysis on a given stock, including:
   - Key financial ratios
   - Growth rates
   - Valuation metrics
   - Future estimates
   - Simple DCF valuation

To use the agent, simply run the cells in order. You can modify the stock ticker or company name in the function calls to analyze different stocks.

## Examples

**Get recent news about Morgan Stanley:**

stock_news('Morgan Stanley')

**Perform fundamental analysis on Intel: **

stock_financial('intel')



## Note

This project is for educational purposes only. Always do your own research and consult with a financial advisor before making investment decisions.

## License

[MIT License](LICENSE)