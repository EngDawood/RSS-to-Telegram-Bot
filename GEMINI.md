# Project Overview

This project is a Telegram bot that fetches RSS feeds and sends them to Telegram . It is written in Python and uses the `telethon` library to interact with the Telegram API, `feedparser` to parse RSS feeds, and `tortoise-orm` for database operations. The bot supports multiple users, internationalization, and rich text formatting.

# Building and Running

**1. Installation:**

Install the required dependencies using pip:

```bash

pip install -r requirements.txt

```

**2. Configuration:**

Create a `.env` file by copying the `.env.sample` file and fill in the required values, such as your Telegram API ID, API hash, and bot token.

**3. Running the bot:**

Run the bot using the following command:

```bash
python3 telegramRSSbot.py
```

# Development Conventions

The project uses `black` for code formatting and `flake8` for linting. It also uses `pre-commit` to run these checks before each commit. The code is organized into several modules within the `src` directory, with each module responsible for a specific functionality. The `command` module, for example, handles the bot's commands, while the `parsing` module is responsible for parsing RSS feeds and formatting messages.
