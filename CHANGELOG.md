# Changelog

## 1.4.0 · 2026-11-26

- MCP tools: `search`, `fetch`, `list_articles`, `define_term`, `get_research`, `get_ranking_factors`, `get_checklist`, `find_categories`, `get_changes`, `get_plans`, `audit_business`, `send_feedback`.
- Agent Plugins, Claude, ChatGPT and Codex, Antigravity, Gemini CLI, Cursor, Kiro, Kilo, Cline and Devin packages.
- Install links, MCP Registry manifest and catalog listing copy.

- `get_checklist` отдаёт опубликованный чеклист или шаблон по задаче целиком (51 страница в `/guides`), без темы - список всех.
- `get_ranking_factors` читает опубликованный свод факторов места в картах (`scope=maps`) и попадания в ответы ИИ (`scope=ai_answers`); пока свода нет, говорит это и даёт ближайшие опубликованные страницы.
- `fetch`, `get_research` и новые инструменты отдают markdown страницы и в тексте, и в `structuredContent.body_markdown`: Claude Code и OpenCode передают модели только структуру, Codex - только текст (прогон 26.11).
- Незнакомый параметр - ошибка с верными именами, а не молчание.
- Пустые ответы и незнакомые параметры пишутся в журнал "просили - не получили" (`agents/FEEDBACK.md`).

## 1.2.0 · 2026-11-23

- `find_categories` возвращает категории Google Business Profile для США, дату снимка и отраслевые страницы по теме.
- `send_feedback` принимает отзывы о данных и запросы по желанию пользователя.
- Поиск поднимает страницы с точной формулировкой вопроса в заголовке.
- Страница `/agents` включена в карту сайта и доступна в `fetch`.

## 1.3.0 · 2026-11-25

- `audit_business` запускает аудит с общими лимитами сайта, возвращает ссылку и позволяет проверить готовность по `report_id`.
- Поиск учитывает отдельные слова из текста Markdown, даже если страница содержит только часть запроса.

## Навыки плагина · 2026-11-26

- Три навыка-сценария: неделя владельца профиля, заблокированный профиль, разбор профиля по списку.
- Общий навык `maps-agent` называет нынешние инструменты и ведёт в сценарии.
- Сайт отдаёт навыки для Skills Hub агента Hermes: `/.well-known/skills/index.json` и `/.well-known/skills/<имя>/SKILL.md` (те же файлы, что в плагине).
- `/.well-known/glama.json` - файл сопровождающих каталога Glama; сама заявка - вход на glama.ai, файл в корне репо `maps-agent/mcp` (страница вендора).

## 1.0.0

- Remote MCP server `https://maps-agent.com/mcp`: `search_knowledge`, `get_article`, `list_articles`, `define_term`, `get_research`.
- Claude Code and Cursor plugin with the `maps-agent` skill, Gemini CLI extension, MCP Registry entry.
