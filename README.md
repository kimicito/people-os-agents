<h1 align="center">People OS Agents</h1>
<p align="center"><b>7 ИИ-агентов для HR по всему жизненному циклу сотрудника</b><br>Найм · Онбординг · Компетенции и 9-box · Вознаграждение · Оргдизайн · Кадровый резерв</p>

<p align="center">
  <img src="https://img.shields.io/badge/агентов-7-blue?style=flat-square" alt="agents">
  <img src="https://img.shields.io/badge/Amazon_Quick-ready-FF9900?style=flat-square&logo=amazon&logoColor=white" alt="Amazon Quick">
  <img src="https://img.shields.io/badge/Claude_Skills-ready-191919?style=flat-square&logo=anthropic&logoColor=white" alt="Claude">
  <img src="https://img.shields.io/badge/ChatGPT-ready-412991?style=flat-square&logo=openai&logoColor=white" alt="ChatGPT">
  <img src="https://img.shields.io/badge/язык-русский-green?style=flat-square" alt="ru">
  <img src="https://img.shields.io/badge/license-CC_BY_4.0-lightgrey?style=flat-square" alt="license">
</p>

> *EN: Seven open-source HR agents covering the full employee lifecycle. Prompts are in Russian and work in Amazon Quick, Claude (Skills / Projects / Claude Code) and ChatGPT.*

## Зачем это

Большинство HR-промптов просят модель «быть экспертом» и дальше угадывать. Эти агенты устроены иначе:

- **Работают по методологии.** Воронка найма, STAR-интервью, DISC, 30-60-90, 9-box, Total Rewards, span of control, планирование численности.
- **Показывают расчёт.** Каждая цифра посчитана из данных, а если данных нет, агент прямо говорит, чего не хватает.
- **Не принимают кадровых решений.** Найм, оплата, увольнение и ячейка 9-box всегда остаются за человеком. Защищённые признаки (пол, возраст и т. д.) агенты флагуют, а не учитывают.
- **Отвечают таблицами**, которые можно сразу нести на встречу.

## Агенты

| | Агент | Что делает |
|---|---|---|
| 🧭 | [**People OS Architect**](agents/00-people-os-architect) | Аудит HR-системы по жизненному циклу сотрудника: что должно быть написано, что мерить, где AI заменяет, а где решает человек (SCAN). |
| 🎯 | [**Recruiting Agent**](agents/01-recruiting-agent) | Анализирует воронку найма, готовит структурированные интервью и проверяет вакансии на соответствие EVP. |
| 🚀 | [**Onboarding Agent**](agents/02-onboarding-agent) | Строит план 30-60-90 с проверяемыми целями и подбирает стиль онбординга по поведенческому профилю DISC. |
| 📈 | [**Talent Agent**](agents/03-talent-agent) | Описывает компетенции поведением, а не прилагательными, и готовит честную калибровку 9-box без самосбывающихся ярлыков. |
| 💰 | [**Rewards Agent**](agents/04-rewards-agent) | Разбирает вознаграждение по Total Rewards и схемы мотивации продавцов: внутренняя справедливость, простота формулы, пакет под сегмент. |
| 🏗 | [**Org Design Agent**](agents/05-org-design-agent) | Считает диапазон управляемости и глубину иерархии по оргструктуре и предлагает сценарии, а не решения. |
| 👥 | [**Workforce & Succession Agent**](agents/06-workforce-succession-agent) | Переводит план по выручке в план по людям и строит кадровый резерв по критичным ролям. |

## Как они связаны

Начни с **People OS Architect**: он проводит аудит всей HR-системы и для каждого этапа говорит, к какому агенту идти и какой вопрос задать.

```mermaid
flowchart LR
    A[People OS Architect<br>аудит системы] --> R[Recruiting<br>потребность и отбор]
    A --> O[Onboarding<br>адаптация]
    A --> T[Talent<br>развитие]
    A --> W[Rewards<br>удержание]
    A --> D[Org Design<br>структура]
    A --> S[Workforce & Succession<br>численность и резерв]
```

## Методология

Фреймворки, на которых построены агенты, подробно разобраны на [KZSalesHub](https://kzsaleshub.com) в системе People OS: найм, онбординг, компетенции, вознаграждение и карьерные треки.

## Быстрый старт

1. Открой папку нужного агента в [`agents/`](agents).
2. Скопируй текст из `instructions.md` в свою платформу.
3. Подготовь данные по описанию из `knowledge/README.md` и загрузи их как файлы знаний.

Пошаговые инструкции для Amazon Quick, Claude и ChatGPT: [docs/install.md](docs/install.md).

## Структура репозитория

```
agents/
  00-people-os-architect/
    README.md          описание и примеры запросов
    instructions.md    системный промпт (для Quick, ChatGPT, Claude Projects)
    SKILL.md           тот же агент в формате Claude Skill
    knowledge/         какие данные подготовить для агента
  01-recruiting-agent/
  ...
docs/install.md        установка по платформам
```

## Важно

Агенты помогают готовить материалы и не заменяют HR-специалиста. Перед загрузкой реальных данных сотрудников проверь, что платформа и её настройки соответствуют требованиям твоей компании и законодательства о персональных данных.

## Автор и лицензия

[Руслан Омаров](https://www.linkedin.com/in/ruslanomarov/) · открытое сообщество [KZSalesHub](https://kzsaleshub.com) · [Telegram](https://t.me/KZSalesHub)

Лицензия [CC BY 4.0](LICENSE): можно использовать, менять и распространять, в том числе в коммерческих целях, со ссылкой на источник. Предложения и улучшения приветствуются через Issues и Pull Requests.
