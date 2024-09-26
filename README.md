# TelegramQueryIDFetcher

![TelegramQueryIDFetcher](https://img.shields.io/badge/Telegram-QueryIDFetcher-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Python](https://img.shields.io/badge/Python-3.7%2B-yellow.svg)

TelegramQueryIDFetcher 是一个强大且易于使用的工具，用于从 Telegram 机器人中获取 `query_id`。该项目使用 Pyrogram 库与 Telegram API 进行交互，并通过 WebView 请求获取所需的数据

[![Telegram Channel](https://img.shields.io/badge/Telegram-Channel-red?logo=telegram&logoColor=white)](https://t.me/ScriptFreedom)
[![Telegram Group](https://img.shields.io/badge/Telegram-Group-red?logo=telegram&logoColor=white)](https://t.me/ScriptFreedomGroup)

## 🌟 特性

- 🚀 **创建和管理 Telegram 会话**
- 🔍 **从指定的 Telegram 机器人中获取 `query_id`**
- 💾 **将获取到的 `query_id` 保存到文件中**
- 🤖 **支持多机器人和多会话处理**

## 📋 先决条件

在开始之前，请确保你已经满足以下要求：

- Python 3.7+

## 📦 安装

1. 克隆仓库：

    ```bash
    git clone https://github.com/SaulGoodManC99/TelegramQueryIDFetcher.git
    cd TelegramQueryIDFetcher
    ```

2. 安装依赖：

    ```bash
    pip install -r requirements.txt
    copy .env-example .env
    ```

## ⚙️ 配置


1. 获取 `API_ID` 和 `API_HASH`，可以从 [my.telegram.org](https://my.telegram.org) 获取
2. 或者从我的 Telegram 群组回复 API，有公共 API 可用
3. 编辑.env文件，填写API_ID和API_HASH
## 🚀 使用

1. 运行脚本：

    ```bash
    python auto_get_token.py
    ```

2. 选择相应的操作：

    - **创建会话**：输入你的电话号码和会话名称
    - **使用已有会话**：可以从其他脚本 sessions 文件夹中复制到脚本 sessions 文件夹中使用
    - **选择要获取 query_id 的机器人**：选择一个机器人并批量获取 query_id

3. 自动保存 query_id：

     - **自动保存所有 query_id**：机器人相对应的用户名_token.txt

