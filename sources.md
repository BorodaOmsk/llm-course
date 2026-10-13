[← К оглавлению](README.md)

# Источники курса

Первоисточники, на которые опираются уроки. В уроках их содержание пересказано, дословных цитат нет. Ссылки проверены в октябре 2026 года. Документация вендоров обновляется, поэтому при расхождении верьте актуальной версии по ссылке.

## Как устроены LLM, токены, контекст

- Petrov A. et al. «Language Model Tokenizers Introduce Unfairness Between Languages», NeurIPS 2023. Почему один и тот же текст на разных языках занимает разное число токенов. — https://arxiv.org/abs/2305.15425 (урок 02)
- Liu N. F. et al. «Lost in the Middle: How Language Models Use Long Contexts», 2023, TACL 2024. — https://arxiv.org/abs/2307.03172 (уроки 02, 05)
- Anthropic, документация о контекстных окнах. — https://platform.claude.com/docs/en/build-with-claude/context-windows (урок 02)

## Галлюцинации

- Kalai A. T., Nachum O., Vempala S. S., Zhang E. (OpenAI). «Why Language Models Hallucinate», сентябрь 2025. — https://arxiv.org/abs/2509.04664 (урок 03)
- Anthropic, «Reduce hallucinations», руководство по снижению галлюцинаций. — https://platform.claude.com/docs/en/test-and-evaluate/strengthen-guardrails/reduce-hallucinations (уроки 03, 07a)

## Промптинг и модели

- Wei J. et al. «Chain-of-Thought Prompting Elicits Reasoning in Large Language Models», 2022. — https://arxiv.org/abs/2201.11903 (урок 04)
- OpenAI, «Reasoning best practices», рекомендации по работе с reasoning-моделями. — https://platform.openai.com/docs/guides/reasoning-best-practices (уроки 03a, 04)
- Руководства по промптингу от OpenAI, Anthropic и Google (Gemini) в официальной документации вендоров (урок 04).

## Стенд: Kilo Code, Open WebUI, vLLM, модели

Документация меняется вместе с версиями. Внешние ссылки — для чтения; на стенде используйте версии, которые утвердил администратор.

- Kilo Code, настройки и файлы `kilo.jsonc`. — https://kilo.ai/docs/getting-started/settings (уроки 00a, 10)
- Kilo Code, свои модели и провайдеры (Custom provider, `limit`, `tool_call`, `{env:...}` только в доверенном конфиге). — https://github.com/Kilo-Org/kilocode/blob/main/packages/kilo-docs/pages/code-with-ai/agents/custom-models.md (урок 00a)
- Kilo Code, автоподтверждение и права инструментов (значения по умолчанию). — https://kilo.ai/docs/getting-started/settings/auto-approving-actions (уроки 00a, 07, 10)
- Kilo Code, права агентов (шаблоны, `.env`, субагенты). — https://kilo.ai/docs/customize/agent-permissions (уроки 08, 10, 11)
- Kilo Code, встроенные агенты code / ask / plan / debug. — https://kilo.ai/docs/basic-usage/using-modes (уроки 07, 07a, 08)
- Kilo Code, свои агенты (файлы `.kilo/agents/*.md`, `steps`, `mode`). — https://kilo.ai/docs/customize/custom-modes (уроки 08, 11)
- Kilo Code, что нового в 2026 (snapshots, Diff Viewer, график задачи, `/review`). — https://docs.kilo.ai/docs/code-with-ai/platforms/vscode/whats-new (уроки 02, 07a, 10a)
- Kilo Code, MCP. — https://docs.kilo.ai/docs/automate/mcp/using-in-kilo-code (урок 09)
- Chatbox, подключение своего провайдера (OpenAI API compatible, API Host, Check). — https://docs.chatboxai.app/en/guides (урок 00a)
- Chatbox, локальная база знаний. — https://docs.chatboxai.app/en/guides/knowledge-base (урок 06)
- Chatbox, MCP. — https://docs.chatboxai.app/en/guides/mcp (урок 09)
- Chatbox, Work Mode (агентный режим, согласие перед изменениями, пауза каждые 25 шагов). — https://chatboxai.app/en/blog/work-mode-launch (уроки 07, 11)
- Chatbox, где хранятся данные. — https://docs.chatboxai.app/en/faq/faq/data-storage (уроки 00a, 10)
- Chatbox, исходный код. — https://github.com/chatboxai/chatbox
- Open WebUI, работа без интернета (`OFFLINE_MODE` не блокирует сеть). — https://docs.openwebui.com/tutorials/maintenance/offline-mode/ (уроки 00a, 10)
- Open WebUI, базы знаний. — https://docs.openwebui.com/features/workspace/knowledge/ (урок 06)
- Open WebUI, MCP (Streamable HTTP, только администратор, mcpo). — https://docs.openwebui.com/features/extensibility/mcp/ (урок 09)
- vLLM, OpenAI-совместимый сервер и `/tokenize`. — https://docs.vllm.ai/en/stable/serving/openai_compatible_server/ (урок 02)
- vLLM, вызов инструментов (`--enable-auto-tool-choice`, `--tool-call-parser`). — https://docs.vllm.ai/en/stable/features/tool_calling/ (уроки 06, 11)
- vLLM, рассуждения reasoning-моделей (`--reasoning-parser`). — https://docs.vllm.ai/en/stable/features/reasoning_outputs/ (урок 03a)
- Qwen, документация (режимы размышлений, `enable_thinking`). — https://qwen.readthedocs.io (урок 03a)
- Продвинутый материал этого репозитория: [Инфраструктура vLLM](../ai-agents-sdlc/04-vllm-infrastructure.md).

## Контекст и файлы правил

- AGENTS.md, открытый формат файла правил для агентов. — https://agents.md (урок 05)
- Kilo Code, AGENTS.md. — https://docs.kilo.ai/docs/customize/agents-md (урок 05)
- Kilo Code, Custom Rules. — https://kilo.ai/docs/customize/custom-rules (урок 05)

## Знания и инструменты

- Lewis P. et al. «Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks», NeurIPS 2020. — https://arxiv.org/abs/2005.11401 (урок 06)
- OpenAI, документация Function calling. — https://platform.openai.com/docs/guides/function-calling (уроки 06, 11)

## Агенты и паттерны

- Schluntz E., Zhang B. (Anthropic). «Building Effective Agents», декабрь 2024. Определения workflow и агента, пять паттернов, совет начинать с простого. — https://www.anthropic.com/engineering/building-effective-agents (уроки 07, 08, 10a)
- Yao S. et al. «ReAct: Synergizing Reasoning and Acting in Language Models», октябрь 2022, ICLR 2023. — https://arxiv.org/abs/2210.03629 (урок 07)
- Kilo Code, документация по режимам (агентам) и субагентам. — https://kilo.ai/docs/basic-usage/using-modes (урок 08)

## MCP

- Anthropic, «Introducing the Model Context Protocol», 25 ноября 2024. — https://www.anthropic.com/news/model-context-protocol (урок 09)
- Model Context Protocol, официальный сайт. — https://modelcontextprotocol.io (урок 09)
- Каталог MCP-серверов (для чтения; в контуре серверы ставит администратор). — https://github.com/modelcontextprotocol/servers (урок 09)
- Linux Foundation, объявление о создании Agentic AI Foundation, 9 декабря 2025. — https://www.linuxfoundation.org/press/linux-foundation-announces-the-formation-of-the-agentic-ai-foundation (уроки 05, 09)

## Безопасность

- OWASP Top 10 for LLM Applications 2025. — https://genai.owasp.org/resource/owasp-top-10-for-llm-applications-2025/ (урок 10)
- OWASP LLM01:2025 Prompt Injection. — https://genai.owasp.org/llmrisk/llm01-prompt-injection/ (урок 10)
- OWASP LLM06:2025 Excessive Agency. — https://genai.owasp.org/llmrisk/llm062025-excessive-agency/ (урок 10)
- Willison S. «The lethal trifecta for AI agents», июнь 2025. — https://simonwillison.net/2025/Jun/16/the-lethal-trifecta/ (уроки 10, 12)
- mcp-atlassian, MCP-сервер для Jira и Confluence (Server/Data Center, PAT). — https://github.com/sooperset/mcp-atlassian (урок 09)
- GitHub Security Advisory GHSA-3r68-hf9h-887v: обход фильтра `ENABLED_TOOLS` в mcp-atlassian. — https://github.com/sooperset/mcp-atlassian/security/advisories/GHSA-3r68-hf9h-887v (урок 10)

## Фреймворки (ориентир, урок 11)

- LangChain / LangGraph 1.0, октябрь 2025. — https://blog.langchain.com/langchain-langgraph-1dot0/
- OpenAI Agents SDK, март 2025. — https://openai.com/index/new-tools-for-building-agents/
- Microsoft Agent Framework. — https://devblogs.microsoft.com/agent-framework/

---

[← Вернуться к оглавлению](README.md)
