# TelegramQueryIDFetcher

![TelegramQueryIDFetcher](https://img.shields.io/badge/Telegram-QueryIDFetcher-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Python](https://img.shields.io/badge/Python-3.7%2B-yellow.svg)

TelegramQueryIDFetcher is a powerful and easy-to-use tool for retrieving `query_id` from Telegram bots. This project uses the Pyrogram library to interact with the Telegram API and obtains the required data through WebView requests.

[![Telegram Channel](https://img.shields.io/badge/Telegram-Channel-red?logo=telegram&logoColor=white)](https://t.me/ScriptFreedom)
[![Telegram Group](https://img.shields.io/badge/Telegram-Group-red?logo=telegram&logoColor=white)](https://t.me/ScriptFreedomGroup)

[English](#english) | [中文](README_Cn.md) | [Русский](README_Ru.md)

## 🌟 Features

- 🚀 **Create and manage Telegram sessions**
- 🔍 **Retrieve `query_id` from specified Telegram bots**
- 💾 **Save retrieved `query_id` to files**
- 🤖 **Support for multiple bots and multiple sessions**
- 🌐 **Proxy support for enhanced accessibility**

## 📋 Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.7+

## 📦 Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/YourUsername/TelegramQueryIDFetcher.git
    cd TelegramQueryIDFetcher
    ```

2. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

3. Set up your configuration:

    ```bash
    cp .env-example .env
    ```

## ⚙️ Configuration

1. Obtain `API_ID` and `API_HASH` from [my.telegram.org](https://my.telegram.org)
2. Or reply with "API" in our Telegram group for public API credentials
3. Edit the `.env` file and fill in your `API_ID` and `API_HASH`

## 🚀 Usage

1. Run the script:

    ```bash
    python auto_get_token.py
    ```

   For proxy support:

    ```bash
    python auto_get_token_proxy.py
    ```

2. Choose the appropriate action:

    - **Create a session**: Enter your phone number and session name
    - **Use existing sessions**: Copy session files from other scripts' sessions folder to this script's sessions folder
    - **Select a bot to retrieve query_id**: Choose a bot and batch retrieve query_ids

3. Automatic query_id saving:

    - **All query_ids are automatically saved**: in `botusername_token.txt` files

## 🌐 Proxy Support

When using `auto_get_token_proxy.py`, the script will use proxies from the `proxy.txt` file. If the number of proxies is less than the number of sessions, proxies will be reused.

