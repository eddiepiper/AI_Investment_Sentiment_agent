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
git clone https://github.com/eddiepiper/AI_Investment_Sentiment_agent.git
cd AI_Investment_Sentiment_agent
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

   **Important**: Never commit your `.env` file or share your API keys publicly!

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
