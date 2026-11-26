# Changelog

## 1.3.0 · 2026-11-25

- MCP tools: `search`, `fetch`, `list_articles`, `define_term`, `get_research`, `find_categories`, `get_changes`, `get_plans`, `audit_business`, `send_feedback`.
- Agent Plugins, Claude, ChatGPT and Codex, Antigravity, Gemini CLI, Cursor, Kiro, Kilo, Cline and Devin packages.
- Install links, MCP Registry manifest and catalog listing copy.

- `audit_business` запускает аудит с общими лимитами сайта, возвращает ссылку и позволяет проверить готовность по `report_id`.
- Поиск учитывает отдельные слова из текста Markdown, даже если страница содержит только часть запроса.

## 1.2.0 · 2026-11-23

- `find_categories` возвращает категории Google Business Profile для США, дату снимка и отраслевые страницы по теме.
- `send_feedback` принимает отзывы о данных и запросы по желанию пользователя.
- Поиск поднимает страницы с точной формулировкой вопроса в заголовке.
- Страница `/agents` включена в карту сайта и доступна в `fetch`.

## 1.0.0

- Remote MCP server `https://maps-agent.com/mcp`: `search_knowledge`, `get_article`, `list_articles`, `define_term`, `get_research`.
- Claude Code and Cursor plugin with the `maps-agent` skill, Gemini CLI extension, MCP Registry entry.
