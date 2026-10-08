# Установка агентов

Каждый агент лежит в своей папке в `agents/`. Внутри три вещи: `instructions.md` (системный промпт), `SKILL.md` (формат Claude Skill) и папка `knowledge/` с описанием данных для агента.

## Amazon Quick

1. Открой **Chat agents → Create chat agent → Blank**.
2. Впиши имя и описание из `README.md` агента.
3. В блоке **Agent persona → Instructions** вставь содержимое `instructions.md`.
4. В **Reference documents** загрузи документы своей компании (до 10 файлов .md, .pdf, .txt, .docx). Что подготовить, описано в `knowledge/README.md`.
5. По желанию подключи **Knowledge sources** (Spaces) с реальными данными компании.
6. Нажми **Update preview**, проверь на примерах запросов и затем **Launch chat agent**.

## Claude

**Вариант 1. Skill (claude.ai).** Скачай папку агента, упакуй её в zip так, чтобы `SKILL.md` был внутри папки, и загрузи через Settings → Capabilities → Skills. Claude сам подключит навык, когда вопрос подходит под описание.

**Вариант 2. Project.** Создай Project, вставь `instructions.md` в Project instructions, а документы компании загрузи в Project knowledge.

**Вариант 3. Claude Code.** Скопируй папку агента в `~/.claude/skills/<имя-агента>/` (или в `.claude/skills/` внутри проекта).

## ChatGPT

1. **Explore GPTs → Create → Configure**.
2. `instructions.md` вставь в **Instructions**.
3. Документы компании загрузи в **Knowledge**.
4. Добавь примеры запросов из `README.md` агента в **Conversation starters**.

## Другие платформы

`instructions.md` — обычный системный промпт. Он подойдёт для любой модели или фреймворка агентов (API, n8n, LangChain, Bedrock Agents): передай его как system prompt, а документы подключи как контекст или базу знаний.
