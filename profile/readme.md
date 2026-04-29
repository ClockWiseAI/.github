<div align="center">

# 🕒 ClockWise AI

### *Искусственный интеллект, который считает ваше время*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Rust](https://img.shields.io/badge/Rust-1.75+-orange.svg)](https://www.rust-lang.org)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://python.org)
[![Vue](https://img.shields.io/badge/Vue-3.4+-green.svg)](https://vuejs.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.100+-teal.svg)](https://fastapi.tiangolo.com)

*Автоматический трекинг рабочего времени без ручного ввода для российского бизнеса*

</div>

---

## 📦 Репозитории организации

| Репозиторий | Описание | Стек |
|-------------|----------|------|
| [**web**](https://github.com/clockwiseai/web) | Веб-приложение + API | Vue 3, FastAPI, PostgreSQL |
| [**desktop**](https://github.com/clockwiseai/desktop) | Десктоп трекер | Tauri (Rust), React/TS |
| [**ai-engine**](https://github.com/clockwiseai/ai-engine) | AI классификация времени | PyTorch, ONNX, FastAPI |
| [**docs**](https://github.com/clockwiseai/docs) | Документация | Markdown, MKDocs |
| [**infra**](https://github.com/clockwiseai/infra) | Инфраструктура как код | Terraform, Ansible |
| [**mobile**](https://github.com/clockwiseai/mobile) | Мобильное приложение (roadmap) | Kotlin/Swift |

---

## 🎯 О продукте

**ClockWise AI** — B2B SaaS платформа для автоматического учёта рабочего времени с использованием искусственного интеллекта.

### Проблема, которую мы решаем

Сотрудники тратят **до 10 часов в месяц** на ручное заполнение таймшитов. Менеджеры теряют **до 20% биллинга** из-за неучтённых часов.

### Наше решение

- 🤖 **Полная автоматизация** — ИИ сам определяет, над чем работает сотрудник
- 🎯 **99% точности** — обученная модель учитывает контекст и проекты
- 🔌 **Интеграции** — Jira, Asana, Trello, 1С, Битрикс24
- 🇷🇺 **Работа в РФ** — сервера в России, поддержка импортозамещённого ПО
- 🔒 **Безопасность** — 152-ФЗ, шифрование данных, on-premise опция

---

## 🏗️ Архитектура

```
┌─────────────────────────────────────────────────────────────┐
│                    Desktop App (Tauri)                      │
│  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐   │
│  │Windows   │  │macOS     │  │Linux     │  │Browser   │   │
│  │Native    │  │Native    │  │X11/Wayland│  │Extension │   │
│  └────┬─────┘  └────┬─────┘  └────┬─────┘  └────┬─────┘   │
└───────┼─────────────┼─────────────┼─────────────┼─────────┘
        │             │             │             │
        └─────────────┴─────────────┴─────────────┘
                          │ WebSocket / REST
        ┌─────────────────▼─────────────────┐
        │         API Gateway (FastAPI)      │
        └─────────────────┬─────────────────┘
                          │
        ┌─────────────────┼─────────────────┐
        │                 │                 │
   ┌────▼────┐       ┌─────▼──────┐    ┌─────▼──────┐
   │PostgreSQL│       │  Redis     │    │  ClickHouse│
   │(users,   │       │(queue,     │    │ (analytics,│
   │projects) │       │  cache)    │    │  metrics)  │
   └──────────┘       └────────────┘    └────────────┘
                          │
                   ┌──────▼───────┐
                   │  AI Engine   │
                   │ (PyTorch/    │
                   │  ONNX)       │
                   └──────────────┘
```

---

## 🚀 Быстрый старт для разработчика
Пока-что не предусмотрен

---

## 📊 Текущий статус

| Компонент | Статус | Coverage | Производительность |
|-----------|--------|----------|---------------------|
| Web API | ⚪ Planned | — | — |
| Desktop App | ⚪ Planned | — | — |
| AI Engine | ⚪ Planned | — | — |
| Mobile App | ⚪ Planned | — | — |

**Roadmap:**
- 📅 Q1 2027: Прототип AI классификации
- 📅 Q2 2027: MVP веб-приложения
- 📅 Q3 2027: Десктоп трекер (текущая фаза)
- 📅 Q4 2027: Интеграция с 1С
- 📅 Q1 2028: On-premise версия

---

## 🔗 Полезные ссылки

| | |
|---|---|
| 🌐 **Веб-сайт** | [clockwise.ai]() |
| 📖 **Документация** | [docs.clockwise.ai]() |
| 💬 **Telegram чат** | [t.me/clockwise_ai]() |
| 🐛 **Баги и фичи** | [Issues]() |
| 📧 **Поддержка** | [support@clockwise.ai]() |
| 🇷🇺 **Российский офис** | В скором времени |

---

## 📄 Лицензия

```
Copyright © 2026 ClockWise AI

Программное обеспечение ClockWise AI распространяется под двойной лицензией:
- Исходный код сообщества: MIT License
- Коммерческая версия: Proprietary License

Подробнее в файле LICENSE
```

---

<div align="center">

**⭐ Звездите репозиторий, если ClockWise AI помогает вам управлять временем!**

*Сделано с ❤️ в России*

</div>
