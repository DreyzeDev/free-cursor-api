# ⚡ Free OpenAI & Cursor API — 50,000,000 Tokens Welcome Grant

[![SnakesRouter Channel](https://img.shields.io/badge/Telegram-Channel-blue?logo=telegram)](https://t.me/SnakesRouters)
[![SnakesRouter Bot](https://img.shields.io/badge/Telegram-Get_Key-2BA6E1?logo=telegram)](https://t.me/SnakesRouterBot)
[![Status](https://img.shields.io/badge/Status-Operational-brightgreen)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **High-speed, enterprise-grade AI gateway powered by Microsoft Azure OpenAI (East US 2).**  
> Access authentic frontier reasoning (`snakes-astra`), high-throughput coding (`snakes-sol`), and rapid reasoning (`snakes-6.1`) models with **50,000,000 welcome tokens**!

[English](#-english-guide) | [Русский](#-инструкция-на-русском)

---

## 🇷🇺 Инструкция на русском

### 🚀 Что это такое?
**SnakesRouter** — это высокоскоростной шлюз к оригинальным моделям OpenAI, работающим на корпоративной облачной инфраструктуре **Microsoft Azure OpenAI (кластер East US 2)**.

- **100% Оригинальные веса:** настоящий Test-Time Compute (скрытые reasoning-токены CoT), оригинальный BPE токенизатор `o200k_base`.
- **Без посредников и урезаний:** полный контекст, отсутствие цензурных заглушек на валидный код.
- **Бесплатный стартовый грант:** **50,000,000 токенов** каждому новому разработчику!

### 🧠 Доступные модели
| Модель | Алиас | Назначение |
|---|---|---|
| `snakes-astra` | `astra` | **Флагманский глубокий reasoning (o-серия)**. Архитектура, математика, олимпиадная логика. |
| `snakes-sol` | `sol` | **Сверхбыстрый workhorse**. Повседневный агентный кодинг, тесты, рефакторинг. |
| `snakes-6.1` | `6.1` | **Скоростная reasoning-модель**. Оптимальный баланс глубины мышления и задержки. |

---

### 💻 Как подключить за 1 минуту

#### 1. Получите персональный API-ключ:
1. Запустите официального Telegram-бота: **[@SnakesRouterBot](https://t.me/SnakesRouterBot)**
2. Подпишитесь на канал обновлений: **[@SnakesRouters](https://t.me/SnakesRouters)**
3. Нажмите кнопку **«🔐 Мой API-ключ»** — бот мгновенно сгенерирует ваш персональный ключ и начислит бонус.

---

#### 2. Настройка в Cursor IDE:
1. Откройте **Settings** в Cursor (`Ctrl + Shift + J` или `Cmd + Shift + J`).
2. Перейдите во вкладку **Models** -> **OpenAI API Key**.
3. Включите галочку **Override OpenAI Base URL** и укажите:
   ```text
   https://snakese.space/v1
   ```
4. Вставьте ваш ключ из бота (`sk-snake-...`).
5. В поле **Model Names** добавьте:
   * `snakes-sol`
   * `snakes-astra`
   * `snakes-6.1`
6. Нажмите **Verify** — готово! Теперь Cursor работает через SnakesRouter.

---

#### 3. Использование в Python:
```python
from openai import OpenAI

client = OpenAI(
    base_url="https://snakese.space/v1",
    api_key="ВАШ_КЛЮЧ_ИЗ_БОТА"
)

response = client.chat.completions.create(
    model="snakes-sol",
    messages=[
        {"role": "user", "content": "Напиши асинхронный HTTP-клиент на aiohttp"}
    ]
)

print(response.choices[0].message.content)
```

#### 4. Использование через cURL:
```bash
curl https://snakese.space/v1/chat/completions \
  -H "Authorization: Bearer ВАШ_КЛЮЧ_ИЗ_БОТА" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "snakes-sol",
    "messages": [{"role": "user", "content": "Привет, мир!"}]
  }'
```

---

## 🇬🇧 English Guide

### 🚀 Overview
**SnakesRouter** provides seamless, low-latency access to Microsoft Azure OpenAI enterprise instances (`East US 2`). Built specifically for coding agents (Cursor, DrCode, Claude Code, Cline, Roo Code), backend services, and developers.

### 🎁 Welcome Bonus
* **50,000,000 free tokens** automatically granted to every newly registered developer via [@SnakesRouterBot](https://t.me/SnakesRouterBot).
* **Referral program:** Earn +5,000,000 monthly tokens for every colleague or developer you invite.

### 🛠 Supported Tools
- **Cursor IDE**
- **DrCode & OpenCode**
- **Claude Code CLI**
- **Cline & Roo Code (VS Code)**
- **OpenAI Python & TypeScript SDKs**
- **LangChain & LlamaIndex**

---

## 🔗 Useful Links & Community
- **Telegram Key Bot:** [@SnakesRouterBot](https://t.me/SnakesRouterBot)
- **News & Model Updates:** [@SnakesRouters](https://t.me/SnakesRouters)
- **Web Dashboard:** [https://snakese.space/app/](https://snakese.space/app/)

---
*MIT License — Made for the developer community.*
