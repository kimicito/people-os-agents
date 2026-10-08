# 🎯 Recruiting Agent

Анализирует воронку найма, готовит структурированные интервью и проверяет вакансии на соответствие EVP.

*EN: Hiring funnel analysis, structured interview guides with scoring anchors, EVP check of job ads.*

## Что умеет

Полная логика агента описана в [`instructions.md`](instructions.md). Агент работает по методологии, показывает расчёты и всегда оставляет решение за человеком.

## Методология

Подключи к агенту справочные документы:

- [`recruitment-funnel.md`](../../methodology/ru/recruitment-funnel.md)
- [`structured-interview.md`](../../methodology/ru/structured-interview.md)
- [`evp.md`](../../methodology/ru/evp.md)
- [`competency-model.md`](../../methodology/ru/competency-model.md)

**English:** [`instructions.en.md`](instructions.en.md) · Claude Skill: [`skills-en/recruiting-agent-en`](../../skills-en/recruiting-agent-en)

## Примеры запросов

- Вот выгрузка воронки по вакансии Sales Manager. Где узкое место?
- Собери гайд структурированного интервью для Middle Account Executive.
- Перепиши эту вакансию без «дружного коллектива».

## Какие данные нужны

Подробно описано в [`knowledge/README.md`](knowledge/README.md). Данные компании, которые подключались в исходной версии агента:

- competency_model.md — модель компетенций по уровням
- recruiting_funnel_data.md — данные воронки

Подставь вместо них документы своей компании.

## Установка

| Платформа | Как подключить |
|---|---|
| **Amazon Quick** | Chat agents → Create chat agent → Blank. В поле *Instructions* вставь текст из `instructions.md`, в *Reference documents* загрузи документы компании |
| **Claude (claude.ai)** | Скачай папку агента zip-архивом и загрузи в Settings → Capabilities → Skills. Или создай Project и вставь `instructions.md` в инструкции проекта |
| **Claude Code** | Скопируй папку в `~/.claude/skills/recruiting-agent/` |
| **ChatGPT** | Explore GPTs → Create → Configure. `instructions.md` в Instructions, документы компании в Knowledge |

Подробнее: [docs/install.md](../../docs/install.md)
