# Stock Market AI Agent

This project implements an AI agent that can fetch and analyze stock market data based on natural language queries. It uses LangChain, OpenAI, and FastAPI to create a powerful and flexible API.

## Features

- Natural language processing for stock market queries
- Real-time stock price and information retrieval
- RESTful API for easy integration
- Detailed stock information including price, volume, market cap, etc.

## Requirements

- Python 3.9+
- OpenAI API key

## Installation

1. Clone this repository:
git clone [https://github.com/yourusername/stock-market-agent.git](https://github.com/yourusername/stock-market-agent.git)
cd stock-market-agent

2. Install dependencies:
pip install -r requirements.txt

3. Run the application:
uvicorn main:app --reload


The API will be available at `http://localhost:8000`.

## API Usage

### Query Endpoint

POST /query


Request body:
```json
{
  "query": "What is the current price of AAPL?",
  "openai_api_key": "your-openai-api-key"
}

Response:
{
  "response": "The current price of Apple Inc. (AAPL) is $178.72. The stock opened at $177.23 today, with a day high of $179.15 and a day low of $176.45. The previous close was $177.97. The trading volume is 59,907,200 and the market cap is $2.8 trillion."
}

## Deployment

### Using Docker

1. Build the Docker image:
docker build -t stock-market-agent .

2. Run the container:
docker run -p 8000:8000 stock-market-agent

### Deploying to Heroku

1. Login to Heroku:

```plaintext
heroku login
```


2. Create a new Heroku app:

```plaintext
heroku create your-app-name
```


3. Push to Heroku:

```plaintext
git push heroku main
```

### Deploying to Heroku

1. Login to Heroku:

```plaintext
heroku login
```


2. Create a new Heroku app:

```plaintext
heroku create your-app-name
```


3. Push to Heroku:

```plaintext
git push heroku main
```