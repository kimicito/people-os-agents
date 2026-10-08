# 👥 Workforce & Succession Agent

Переводит план по выручке в план по людям и строит кадровый резерв по критичным ролям.

*EN: Turns a revenue plan into a headcount plan and builds succession pipelines for critical roles.*

## Что умеет

Полная логика агента описана в [`instructions.md`](instructions.md). Агент работает по методологии, показывает расчёты и всегда оставляет решение за человеком.

## Методология

Подключи к агенту справочные документы:

- [`workforce-planning.md`](../../methodology/ru/workforce-planning.md)
- [`succession-planning.md`](../../methodology/ru/succession-planning.md)

**English:** [`instructions.en.md`](instructions.en.md) · Claude Skill: [`skills-en/workforce-succession-agent-en`](../../skills-en/workforce-succession-agent-en)

## Примеры запросов

- План на год — 2 млн $ выручки. Сколько людей нужно в продажах, пресейле и внедрении?
- Построй карту преемников по критичным ролям.

## Какие данные нужны

Подробно описано в [`knowledge/README.md`](knowledge/README.md). Данные компании, которые подключались в исходной версии агента:

- workforce_succession.md — данные для расчёта численности и резерва

Подставь вместо них документы своей компании.

## Установка

| Платформа | Как подключить |
|---|---|
| **Amazon Quick** | Chat agents → Create chat agent → Blank. В поле *Instructions* вставь текст из `instructions.md`, в *Reference documents* загрузи документы компании |
| **Claude (claude.ai)** | Скачай папку агента zip-архивом и загрузи в Settings → Capabilities → Skills. Или создай Project и вставь `instructions.md` в инструкции проекта |
| **Claude Code** | Скопируй папку в `~/.claude/skills/workforce-succession-agent/` |
| **ChatGPT** | Explore GPTs → Create → Configure. `instructions.md` в Instructions, документы компании в Knowledge |

Подробнее: [docs/install.md](../../docs/install.md)
