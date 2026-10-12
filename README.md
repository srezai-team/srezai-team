<!-- Кладётся в публичный репозиторий `srezai-team/srezai-team` как README.md:
     GitHub показывает его на странице профиля. Имя репозитория обязано совпадать
     с именем аккаунта, иначе README на профиле не появится. -->

# срезAI (srezai) - MCP-сервер для веб-поиска и чтения страниц

**Веб-доступ для ИИ-агентов: поиск в интернете, чтение страниц в чистый Markdown
и извлечение данных по схеме — 12 инструментов через MCP (Model Context Protocol),
сильное покрытие рунета, оплата за результат вместо подписки.**

- **MCP-сервер (remote):** `https://srezai.ru/api/mcp` — Streamable HTTP, ключ в заголовке `Authorization: Bearer` · [документация](https://srezai.ru/docs/mcp)
- **API-ключи и баланс:** [srezai.ru/dashboard](https://srezai.ru/dashboard)
- **Официальный реестр MCP:** запись `ru.srezai/search` — [проверить версии](https://registry.modelcontextprotocol.io/v0/servers/ru.srezai%2Fsearch/versions)
- **Каталоги:** [Smithery](https://smithery.ai/servers/srezai/srezai-search) · [Glama](https://glama.ai/mcp/servers/srezai-team/srezai-mcp)

## Репозитории

| Что | Где |
|---|---|
| MCP-сервер, stdio-мост (MIT) | [srezai-mcp-web-search](https://github.com/srezai-team/srezai-mcp-web-search) |
| SDK: Python и JS/TypeScript | [srezai-web-search-sdk](https://github.com/srezai-team/srezai-web-search-sdk) |
| Узел для n8n (автоматизация без кода) | [n8n-nodes-srezai](https://github.com/srezai-team/n8n-nodes-srezai) |
| Скилл для Claude Code и DSH | [srezai-web-search-pro-skill](https://github.com/srezai-team/srezai-web-search-pro-skill) |
| Зеркало на GitVerse | [gitverse.ru/a1_ai_a4b/srezai-mcp](https://gitverse.ru/a1_ai_a4b/srezai-mcp) |

## Двенадцать инструментов

`web_search` — поиск в вебе (до 30 результатов, фильтры по домену, языку, свежести) ·
`image_search` · `read_url` — страница в Markdown, с рендером JavaScript ·
`read_urls` — пачка страниц разом · `fetch_page` — полноценный браузер и скриншот ·
`extract` — поля по JSON-схеме · `map` и `crawl` — карта сайта и обход раздела ·
`verify_claim` — проверка утверждения с дословными цитатами ·
`answer_search` и `deep_research` — готовый ответ по источникам ·
`get_usage` — баланс и квоты, бесплатно

## С чего начать

```bash
# MCP: локальный мост к remote-серверу (ключ берётся в личном кабинете)
npx -y srezai-mcp
```

```bash
pip install srezai      # Python SDK
npm install srezai      # JS/TypeScript SDK
```

## Частые вопросы

**Что такое срезAI (srezai)?** Сервис веб-доступа для ИИ-агентов: он ищет в
интернете, открывает страницы полноценным браузером, отдаёт текст в Markdown и
извлекает нужные поля по схеме — по протоколу MCP, из любого клиента (Claude,
Cursor, n8n и другие).

**Чем это отличается от обычного поиска?** Агенту нужен текст, а не десять синих
ссылок: страница приходит уже очищенной, окнами под размер контекста, а данные
можно запросить полями. Оплата — за фактически выполненный вызов, а не подписка.

**Почему «сильное покрытие рунета»?** Русскоязычные источники — суды, госсайты,
отраслевые реестры, региональные СМИ — обычные западные поисковики обходят плохо.
Это наша сильная сторона: запросы на русском работают предсказуемо.

**Нужен ли ключ?** Да, ключ создаётся в личном кабинете; проверка баланса
(`get_usage`) бесплатна. Стартовый бонус начисляется после подтверждения Telegram.

**Сколько инструментов?** Двенадцать MCP-инструментов; список и цены сервер отдаёт
сам, поэтому в клиентских пакетах они не дублируются.

---

## English

**Web access for AI agents** — web search, page reading as clean Markdown and
schema-based extraction, exposed as **12 MCP (Model Context Protocol) tools**, with
strong Russian-web coverage and pay-per-result pricing instead of a subscription.

- **Remote MCP server:** `https://srezai.ru/api/mcp` — Streamable HTTP, API key via `Authorization: Bearer` · [docs](https://srezai.ru/docs/mcp)
- **API keys & balance:** [srezai.ru/dashboard](https://srezai.ru/dashboard)
- **Official MCP Registry entry:** `ru.srezai/search` — [versions](https://registry.modelcontextprotocol.io/v0/servers/ru.srezai%2Fsearch/versions)
- **Catalogs:** [Smithery](https://smithery.ai/servers/srezai/srezai-search) · [Glama](https://glama.ai/mcp/servers/srezai-team/srezai-mcp)

### Repositories

| What | Where |
|---|---|
| MCP server, stdio bridge (MIT) | [srezai-mcp-web-search](https://github.com/srezai-team/srezai-mcp-web-search) |
| SDK: Python and JS/TypeScript | [srezai-web-search-sdk](https://github.com/srezai-team/srezai-web-search-sdk) |
| n8n community node | [n8n-nodes-srezai](https://github.com/srezai-team/n8n-nodes-srezai) |
| Skill for Claude Code and DSH | [srezai-web-search-pro-skill](https://github.com/srezai-team/srezai-web-search-pro-skill) |
| GitVerse mirror | [gitverse.ru/a1_ai_a4b/srezai-mcp](https://gitverse.ru/a1_ai_a4b/srezai-mcp) |

### Twelve tools

`web_search` · `image_search` · `read_url` · `read_urls` · `fetch_page` · `extract`
· `verify_claim` · `answer_search` · `deep_research` · `map` · `crawl` · `get_usage`

### Get started

```bash
npx -y srezai-mcp      # MCP bridge (MIT), key from the dashboard
pip install srezai     # Python SDK
npm install srezai     # JS/TypeScript SDK
```

---

🌐 [srezai.ru](https://srezai.ru) · ✉️ support@srezai.ru · 💬 [Telegram](https://t.me/srezai_ru) · [VK](https://vk.ru/srezai_ru)
