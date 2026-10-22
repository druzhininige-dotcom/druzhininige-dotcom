# Артём Дружинин

**Автоматизация бизнеса, ИИ-агенты, Telegram-боты, Python.**

Строю системы, которые считают деньги и снимают ручную работу — от сметы для мебельного цеха
до радара лидов по Telegram-чатам. Не «демо нейросети», а то, чем пользуются каждый день.

![Python](https://img.shields.io/badge/Python-3.11-3776AB?logo=python&logoColor=white)
![Telegram](https://img.shields.io/badge/Telegram-Bot%20API-26A5E4?logo=telegram&logoColor=white)
![LLM](https://img.shields.io/badge/LLM-agents-412991?logo=openai&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-n8n-2496ED?logo=docker&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-pytest-003B57?logo=sqlite&logoColor=white)

---

## Чем занимаюсь

- **ИИ-агенты** — пайплайны «сообщение → предфильтр → LLM → детерминированный скоринг → карточка менеджеру»
- **Telegram-боты** — приём файлов, расчёты, отчёты, доставка готовых документов
- **Автоматизация расчётов** — сметы, раскрой, себестоимость: формулы в коде, а не «примерно»
- **Маркетплейсы** — аналитика WB/Ozon через API с защитой от лимитов и блокировок

## Проекты

| Проект | Что решает |
|---|---|
| [Бот смет для мебельного цеха](https://github.com/druzhininige-dotcom/hermes-practice-portfolio/tree/main/01-telegram-bot-smeta) | Раскрой из PRO100 → готовый `.xlsx` на 9 листов прямо из Telegram |
| [Аналитика Wildberries / Ozon](https://github.com/druzhininige-dotcom/hermes-practice-portfolio/tree/main/02-marketplace-analytics) | Экономика по артикулам, воронка, отзывы; предохранитель от блокировок API |
| [3D-конфигуратор мебели](https://github.com/druzhininige-dotcom/hermes-practice-portfolio/tree/main/03-furniture-3d-configurator) | Параметры → 3D-сцена + раскрой + смета по прайсу цеха |
| [Lid_AI — радар лидов](https://github.com/druzhininige-dotcom/hermes-practice-portfolio/tree/main/04-lid-ai) | Сообщения из чатов → оценка по 4 профилям услуг → карточка лида |
| [Голосовой ассистент](https://github.com/druzhininige-dotcom/hermes-practice-portfolio/tree/main/05-family-voice-assistant) | Расписание, будильник и напоминания голосом |

**Все проекты с исходным кодом:** [hermes-practice-portfolio](https://github.com/druzhininige-dotcom/hermes-practice-portfolio)

## Как я работаю

**Деньги считает код, а не модель.** В сметах, раскрое и себестоимости нет вызовов LLM —
только формулы и прайс. Нейросеть там, где нужна семантика: распознать деталь, понять, лид это или нет.

**Нет данных — нет числа.** Если цены нет в прайсе, в документе появляется `УТОЧНИТЬ`,
а не правдоподобная цифра. Каждое допущение выводится отдельным листом.

**Лимиты площадок — часть архитектуры.** Wildberries блокирует по IP, отвечая не `429`,
а обрывом TLS. Поэтому все запросы идут через один клиент с интервалами и остановкой.

---

Открыт к задачам: автоматизация процессов, ИИ-агенты, интеграции, Telegram-боты.
