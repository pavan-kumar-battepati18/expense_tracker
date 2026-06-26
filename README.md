# Personal Finance Tracker 💰

A Python-based CLI expense tracker with real-time Telegram push notifications on every transaction.

## Features
- Add expenses with category and notes
- Add income with sender details
- Instant Telegram notification on every transaction
- CSV based persistent storage
- Daily and total summary with balance calculation

## Tech Stack
Python | Telegram Bot API | REST API | CSV | python-dotenv

## How It Works
1. User adds an expense or income via CLI menu
2. Transaction is saved permanently to a CSV file
3. Instant Telegram push notification is sent to phone
4. Summary shows daily and total balance anytime

## Setup
1. Clone the repo
   git clone https://github.com/pavan-kumar-battepati18/expense_tracker.git

2. Install dependencies
   pip install requests python-dotenv

3. Create a .env file in the project folder
   BOT_TOKEN=your_telegram_bot_token
   CHAT_ID=your_telegram_chat_id

4. Get your Telegram credentials
   - Bot Token → message @BotFather on Telegram
   - Chat ID   → message @userinfobot on Telegram

5. Run the project
   python expense_tracker.py

## Project Structure
expense_tracker/
    expense_tracker.py   → main application
    .env                 → secret tokens (not uploaded)
    expenses.csv         → auto generated on first run
    .gitignore           → hides .env and csv from GitHub
