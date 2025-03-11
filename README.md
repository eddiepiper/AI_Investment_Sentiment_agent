# 💻 Multimodal AI Coding Agent Team with o3-mini and Gemini
An AI Powered Streamlit application that serves as your personal coding assistant, powered by multiple Agents built on the new o3-mini model. You can also upload an image of a coding problem or describe it in text, and the AI agent will analyze, generate an optimal solution, and execute it in a sandbox environment.

## Features
#### Multi-Modal Problem Input
- Upload images of coding problems (supports PNG, JPG, JPEG)
- Type problems in natural language
- Automatic problem extraction from images
- Interactive problem processing

#### Intelligent Code Generation
- Optimal solution generation with best time/space complexity
- Clean, documented Python code output
- Type hints and proper documentation
- Edge case handling

#### Secure Code Execution
- Sandboxed code execution environment
- Real-time execution results
- Error handling and explanations
- 30-second execution timeout protection

#### Multi-Agent Architecture
- Vision Agent (Gemini-2.0-flash) for image processing
- Coding Agent (OpenAI- o3-mini) for solution generation
- Execution Agent (OpenAI) for code running and result analysis
- E2B Sandbox for secure code execution

## How to Run

Follow the steps below to set up and run the application:
- Get an OpenAI API key from: https://platform.openai.com/
- Get a Google (Gemini) API key from: https://makersuite.google.com/app/apikey
- Get an E2B API key from: https://e2b.dev/docs/getting-started/api-key

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Shubhamsaboo/awesome-llm-apps.git
   cd ai_agent_tutorials/ai_coding_agent_o3-mini
   ```

2. **Install the dependencies**
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Streamlit app**
    ```bash
    streamlit run ai_coding_agent_o3.py
    ```

4. **Configure API Keys**
   - Enter your API keys in the sidebar
   - All three keys (OpenAI, Gemini, E2B) are required for full functionality

## Usage
1. Upload an image of a coding problem OR type your problem description
2. Click "Generate & Execute Solution"
3. View the generated solution with full documentation
4. See execution results and any generated files
5. Review any error messages or execution timeouts

# Stock Sentiment Agent 📈

A powerful Telegram bot that provides real-time stock analysis, technical indicators, and AI-powered market insights. The bot combines technical analysis, sentiment analysis from news headlines, and GPT-4 powered market analysis to give you comprehensive stock information.

## Features 🚀

- **Real-time Stock Data**: Get current stock prices and basic information
- **Technical Analysis**: 
  - RSI (Relative Strength Index)
  - SMA (Simple Moving Average) - 50 and 200 days
  - Buy/Sell signals based on technical indicators
- **Sentiment Analysis**:
  - News sentiment analysis using TextBlob
  - Recent news headlines and sources
  - Market trend indicators
- **AI-Powered Insights**:
  - GPT-4 powered market analysis
  - Technical pattern interpretation
  - Risk and opportunity assessment
  - Short-term and long-term outlook

## Prerequisites 📋

- Python 3.9 or higher
- A Telegram Bot Token (obtain from [@BotFather](https://t.me/botfather))
- OpenAI API Key (for GPT-4 analysis)

## Installation 🔧

1. Clone the repository:
```bash
git clone <repository-url>
cd <repository-directory>
```

2. Create and activate a virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

4. Configure environment variables:
   - Create a `.env` file in the project root
   - Add your API keys:
```env
TELEGRAM_TOKEN=your_telegram_bot_token
OPENAI_API_KEY=your_openai_api_key
```

## Usage 🎯

1. Start the bot:
```bash
python stock_sentiment_agent.py
```

2. In Telegram, start a chat with your bot and use these commands:
   - Send a stock ticker (e.g., "AAPL", "GOOGL")
   - Send a company name (e.g., "Apple stock", "Google stock")
   - Use `/start` or `/help` for instructions

## Features in Detail 📊

### Technical Analysis
- **RSI (Relative Strength Index)**: Momentum indicator that measures the speed and magnitude of recent price changes
- **Moving Averages**: 50-day and 200-day SMAs for trend identification
- **Signal Generation**: Automated buy/sell signals based on technical indicator combinations

### Sentiment Analysis
- Analyzes latest news headlines using natural language processing
- Provides sentiment scores and trend indicators
- Includes recent news articles with sources

### AI Analysis
- GPT-4 powered market analysis
- Comprehensive interpretation of technical and fundamental data
- Risk assessment and market outlook
- Potential catalysts and market drivers

## Rate Limiting ⚠️

To prevent API abuse and ensure stable operation:
- 10-second delay between requests
- Maximum 3 retries for failed requests
- Automatic request throttling

## Error Handling 🛠️

The bot includes robust error handling for:
- Network connectivity issues
- API rate limiting
- Invalid stock tickers
- Data availability problems
- Process management

## Contributing 🤝

Contributions are welcome! Please feel free to submit a Pull Request.

## License 📄

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments 🙏

- [python-telegram-bot](https://github.com/python-telegram-bot/python-telegram-bot) for the Telegram bot framework
- [yfinance](https://github.com/ranaroussi/yfinance) for stock data
- [TextBlob](https://textblob.readthedocs.io/) for sentiment analysis
- [OpenAI](https://openai.com/) for GPT-4 powered analysis
- [ta](https://technical-analysis-library-in-python.readthedocs.io/) for technical analysis indicators
