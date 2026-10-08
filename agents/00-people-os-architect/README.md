# 🧭 People OS Architect

Аудит HR-системы по жизненному циклу сотрудника: что должно быть написано, что мерить, где AI заменяет, а где решает человек (SCAN).

*EN: Audits the whole HR system across the employee lifecycle and routes each stage to a specialist agent.*

## Что умеет

Полная логика агента описана в [`instructions.md`](instructions.md). Агент работает по методологии, показывает расчёты и всегда оставляет решение за человеком.

## Примеры запросов

- Проведи аудит нашей HR-системы. Нас 40 человек, есть только оргструктура и положение о премиях.
- Какие 4 HR-метрики нам начать считать в первую очередь?
- Где в нашем найме ИИ может заменить человека, а где нельзя?

## Какие данные нужны

Подробно описано в [`knowledge/README.md`](knowledge/README.md). В исходной версии агента подключались такие документы:

- people_os_company.md — описание компании и текущих HR-процессов

Подставь вместо них документы своей компании.

## Установка

| Платформа | Как подключить |
|---|---|
| **Amazon Quick** | Chat agents → Create chat agent → Blank. В поле *Instructions* вставь текст из `instructions.md`, в *Reference documents* загрузи документы компании |
| **Claude (claude.ai)** | Скачай папку агента zip-архивом и загрузи в Settings → Capabilities → Skills. Или создай Project и вставь `instructions.md` в инструкции проекта |
| **Claude Code** | Скопируй папку в `~/.claude/skills/people-os-architect/` |
| **ChatGPT** | Explore GPTs → Create → Configure. `instructions.md` в Instructions, документы компании в Knowledge |

Подробнее: [docs/install.md](../../docs/install.md)
