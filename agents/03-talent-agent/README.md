# 📈 Talent Agent

Описывает компетенции поведением, а не прилагательными, и готовит честную калибровку 9-box без самосбывающихся ярлыков.

*EN: Rewrites competency models into observable behaviour and prepares fair 9-box calibration materials.*

## Что умеет

Полная логика агента описана в [`instructions.md`](instructions.md). Агент работает по методологии, показывает расчёты и всегда оставляет решение за человеком.

## Методология

Подключи к агенту справочные документы:

- [`competency-model.md`](../../methodology/ru/competency-model.md)
- [`nine-box.md`](../../methodology/ru/nine-box.md)

**English:** [`instructions.en.md`](instructions.en.md) · Claude Skill: [`skills-en/talent-agent-en`](../../skills-en/talent-agent-en)

## Примеры запросов

- Перепиши нашу модель компетенций для продавцов в поведенческие индикаторы.
- Подготовь материалы к калибровке 9-box по этой команде.
- У троих сотрудников нет данных по потенциалу. Что собрать?

## Какие данные нужны

Подробно описано в [`knowledge/README.md`](knowledge/README.md). Данные компании, которые подключались в исходной версии агента:

- competency_model.md — модель компетенций
- ninebox_team.md — данные команды для калибровки

Подставь вместо них документы своей компании.

## Установка

| Платформа | Как подключить |
|---|---|
| **Amazon Quick** | Chat agents → Create chat agent → Blank. В поле *Instructions* вставь текст из `instructions.md`, в *Reference documents* загрузи документы компании |
| **Claude (claude.ai)** | Скачай папку агента zip-архивом и загрузи в Settings → Capabilities → Skills. Или создай Project и вставь `instructions.md` в инструкции проекта |
| **Claude Code** | Скопируй папку в `~/.claude/skills/talent-agent/` |
| **ChatGPT** | Explore GPTs → Create → Configure. `instructions.md` в Instructions, документы компании в Knowledge |

Подробнее: [docs/install.md](../../docs/install.md)
