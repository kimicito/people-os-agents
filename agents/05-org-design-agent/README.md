# 🏗 Org Design Agent

Считает диапазон управляемости и глубину иерархии по оргструктуре и предлагает сценарии, а не решения.

*EN: Calculates span of control and hierarchy layers from an org chart and proposes scenarios, not decisions.*

## Что умеет

Полная логика агента описана в [`instructions.md`](instructions.md). Агент работает по методологии, показывает расчёты и всегда оставляет решение за человеком.

## Примеры запросов

- Посчитай span of control по этой оргструктуре и отметь флаги.
- Предложи 2–3 сценария, как убрать лишний уровень иерархии в продажах.

## Какие данные нужны

Подробно описано в [`knowledge/README.md`](knowledge/README.md). В исходной версии агента подключались такие документы:

- org_structure.md — оргструктура

Подставь вместо них документы своей компании.

## Установка

| Платформа | Как подключить |
|---|---|
| **Amazon Quick** | Chat agents → Create chat agent → Blank. В поле *Instructions* вставь текст из `instructions.md`, в *Reference documents* загрузи документы компании |
| **Claude (claude.ai)** | Скачай папку агента zip-архивом и загрузи в Settings → Capabilities → Skills. Или создай Project и вставь `instructions.md` в инструкции проекта |
| **Claude Code** | Скопируй папку в `~/.claude/skills/org-design-agent/` |
| **ChatGPT** | Explore GPTs → Create → Configure. `instructions.md` в Instructions, документы компании в Knowledge |

Подробнее: [docs/install.md](../../docs/install.md)
