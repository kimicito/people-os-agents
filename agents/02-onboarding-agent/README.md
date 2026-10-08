# 🚀 Onboarding Agent

Строит план 30-60-90 с проверяемыми целями и подбирает стиль онбординга по поведенческому профилю DISC.

*EN: Builds 30-60-90 onboarding plans with verifiable goals and adapts onboarding style to a DISC hypothesis.*

## Что умеет

Полная логика агента описана в [`instructions.md`](instructions.md). Агент работает по методологии, показывает расчёты и всегда оставляет решение за человеком.

## Методология

Подключи к агенту справочные документы:

- [`onboarding-30-60-90.md`](../../methodology/ru/onboarding-30-60-90.md)
- [`disc.md`](../../methodology/ru/disc.md)

**English:** [`instructions.en.md`](instructions.en.md) · Claude Skill: [`skills-en/onboarding-agent-en`](../../skills-en/onboarding-agent-en)

## Примеры запросов

- Составь план 30-60-90 для нового Sales Manager.
- Вот переписка с кандидатом (он согласен на анализ). Какая гипотеза стиля DISC?
- День 30: вот статус по целям. Что дальше?

## Какие данные нужны

Подробно описано в [`knowledge/README.md`](knowledge/README.md). Данные компании, которые подключались в исходной версии агента:

- disc_guide.md — справочник DISC: маркеры и форматы онбординга
- candidate_chat.md — переписка с кандидатом (с его согласия)

Подставь вместо них документы своей компании.

## Установка

| Платформа | Как подключить |
|---|---|
| **Amazon Quick** | Chat agents → Create chat agent → Blank. В поле *Instructions* вставь текст из `instructions.md`, в *Reference documents* загрузи документы компании |
| **Claude (claude.ai)** | Скачай папку агента zip-архивом и загрузи в Settings → Capabilities → Skills. Или создай Project и вставь `instructions.md` в инструкции проекта |
| **Claude Code** | Скопируй папку в `~/.claude/skills/onboarding-agent/` |
| **ChatGPT** | Explore GPTs → Create → Configure. `instructions.md` в Instructions, документы компании в Knowledge |

Подробнее: [docs/install.md](../../docs/install.md)
