# 💰 Rewards Agent

Разбирает вознаграждение по Total Rewards и схемы мотивации продавцов: внутренняя справедливость, простота формулы, пакет под сегмент.

*EN: Total Rewards analysis and sales compensation plan review: internal equity, simple formulas, scenarios.*

## Что умеет

Полная логика агента описана в [`instructions.md`](instructions.md). Агент работает по методологии, показывает расчёты и всегда оставляет решение за человеком.

## Методология

Подключи к агенту справочные документы:

- [`total-rewards.md`](../../methodology/ru/total-rewards.md)
- [`sales-comp-plan.md`](../../methodology/ru/sales-comp-plan.md)

**English:** [`instructions.en.md`](instructions.en.md) · Claude Skill: [`skills-en/rewards-agent-en`](../../skills-en/rewards-agent-en)

## Примеры запросов

- Проверь нашу схему мотивации продавцов и посчитай доход при 70/100/130% плана.
- Хотим открыть вилки зарплат. Что починить до этого?
- Разложи наш пакет по Total Rewards.

## Какие данные нужны

Подробно описано в [`knowledge/README.md`](knowledge/README.md). Данные компании, которые подключались в исходной версии агента:

- rewards_model.md — схема вознаграждения

Подставь вместо них документы своей компании.

## Установка

| Платформа | Как подключить |
|---|---|
| **Amazon Quick** | Chat agents → Create chat agent → Blank. В поле *Instructions* вставь текст из `instructions.md`, в *Reference documents* загрузи документы компании |
| **Claude (claude.ai)** | Скачай папку агента zip-архивом и загрузи в Settings → Capabilities → Skills. Или создай Project и вставь `instructions.md` в инструкции проекта |
| **Claude Code** | Скопируй папку в `~/.claude/skills/rewards-agent/` |
| **ChatGPT** | Explore GPTs → Create → Configure. `instructions.md` в Instructions, документы компании в Knowledge |

Подробнее: [docs/install.md](../../docs/install.md)
