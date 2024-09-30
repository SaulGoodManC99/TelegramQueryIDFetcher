# TelegramQueryIDFetcher

![TelegramQueryIDFetcher](https://img.shields.io/badge/Telegram-QueryIDFetcher-blue.svg)
![许可证](https://img.shields.io/badge/许可证-MIT-green.svg)
![Python](https://img.shields.io/badge/Python-3.7%2B-yellow.svg)

TelegramQueryIDFetcher 是一个强大且易用的工具，用于从 Telegram 机器人获取 `query_id`。该项目使用 Pyrogram 库与 Telegram API 交互，并通过 WebView 请求获取所需数据。

[![Telegram 频道](https://img.shields.io/badge/Telegram-频道-red?logo=telegram&logoColor=white)](https://t.me/ScriptFreedom)
[![Telegram 群组](https://img.shields.io/badge/Telegram-群组-red?logo=telegram&logoColor=white)](https://t.me/ScriptFreedomGroup)

[English](README.md) | [中文](#中文) | [Русский](README_Ru.md)

## 🌟 特性

- 🚀 **创建和管理 Telegram 会话**
- 🔍 **从指定的 Telegram 机器人获取 `query_id`**
- 💾 **将获取的 `query_id` 保存到文件**
- 🤖 **支持多个机器人和多个会话**
- 🌐 **代理支持，提高可访问性**

## 📋 前提条件

在开始之前，请确保您满足以下要求：

- Python 3.7+

## 📦 安装

1. 克隆仓库：

    ```bash
    git clone https://github.com/YourUsername/TelegramQueryIDFetcher.git
    cd TelegramQueryIDFetcher
    ```

2. 安装依赖：

    ```bash
    pip install -r requirements.txt
    ```

3. 设置配置：

    ```bash
    cp .env-example .env
    ```

## ⚙️ 配置

1. 从 [my.telegram.org](https://my.telegram.org) 获取 `API_ID` 和 `API_HASH`
2. 或在我们的 Telegram 群组中回复 "API" 以获取公共 API 凭据
3. 编辑 `.env` 文件并填写您的 `API_ID` 和 `API_HASH`

## 🚀 使用方法

1. 运行脚本：

    ```bash
    python auto_get_token.py
    ```

   对于代理支持：

    ```bash
    python auto_get_token_proxy.py
    ```

2. 选择适当的操作：

    - **创建会话**：输入您的电话号码和会话名称
    - **使用现有会话**：将其他脚本的会话文件夹中的会话文件复制到此脚本的会话文件夹
    - **选择机器人以获取 query_id**：选择一个机器人并批量获取 query_ids

3. 自动保存 query_id：

    - **所有 query_ids 都会自动保存**：保存在 `botusername_token.txt` 文件中

## 🌐 代理支持

使用 `auto_get_token_proxy.py` 时，脚本将使用 `proxy.txt` 文件中的代理。如果代理数量少于会话数量，代理将被重复使用。
