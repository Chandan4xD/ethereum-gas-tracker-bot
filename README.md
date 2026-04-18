# ⛽ Ethereum Gas Tracker Bot

A Telegram bot that monitors Ethereum gas prices in real-time using the Etherscan API V2. Get instant gas readings or set automatic alerts when gas drops below your target.

## Features

- 🔍 Real-time Ethereum gas prices (Low / Medium / High)
- 🚨 Automatic threshold alerts — get notified when gas drops below your target
- 📊 Background monitoring every 60 seconds
- ⚡ Simple Telegram commands, no app needed

## Commands

| Command | Description |
|--------|-------------|
| `/start` | Welcome message and command list |
| `/gas` | Fetch current gas prices instantly |
| `/setalert <gwei>` | Get alerted when gas drops below value |
| `/stopalert` | Cancel your active alert |
| `/status` | Check your current alert setting |

## Tech Stack

- Python 3
- [python-telegram-bot](https://github.com/python-telegram-bot/python-telegram-bot) via requests
- [Etherscan API V2](https://docs.etherscan.io/v2-migration)
- Threading for background monitoring

## Setup

### 1. Clone the repository
```bash
git clone https://github.com/Chandan4xD/ethereum-gas-tracker-bot.git
cd ethereum-gas-tracker-bot
```

### 2. Install dependencies
```bash
pip install requests
```

### 3. Configure API keys

Create a `.env` file or directly set these in `gas_bot.py`:
