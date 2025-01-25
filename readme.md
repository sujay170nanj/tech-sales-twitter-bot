# Tech Sales Twitter Bot

This project is a Twitter bot that tweets out the best sales by percentage in the Amazon electronics category. When tweeted at with a "search term", it replies with the best sale using that search term. The bot provides a link, price drop, percentage, and image. All scraping is performed on camelcamelcamel.com and amazon.com.

## Features

- Tweets the best sales in the Amazon electronics category
- Replies to tweets with the best sale for a given search term
- Provides detailed information including link, price drop, percentage, and image

## Requirements

- Python 3.7+
- Tweepy
- Requests
- BeautifulSoup4

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/tech-sales-twitter-bot.git
    cd tech-sales-twitter-bot
    ```

2. Install the required Python packages:
    ```sh
    pip install tweepy requests beautifulsoup4
    ```

3. Set up your Twitter API credentials:
    - Create a Twitter Developer account and create a new app to get your API keys
    - Replace the placeholders in the Jupyter notebook with your actual Twitter API credentials:
        ```python
        CONSUMER_KEY = 'your_consumer_key'
        CONSUMER_SECRET = 'your_consumer_secret'
        ACCESS_TOKEN = 'your_access_token'
        ACCESS_SECRET = 'your_access_secret'
        ```

## Usage

1. Open the Jupyter notebook `Tech Sales Twitter Bot.ipynb` in Jupyter Notebook or Jupyter Lab

2. Run all the cells in the notebook to start the bot

3. The bot will tweet the best sale once a day and reply to tweets with the best sale for a given search term

## How It Works

- The bot scrapes data from camelcamelcamel.com and amazon.com to find the best sales
- It uses Tweepy to interact with the Twitter API
- The bot tweets the best sales once a day and listens for tweets mentioning it to reply with the best sale for a given search term
