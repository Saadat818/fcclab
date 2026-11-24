# Настройка Claude Code и OpenRouter на macOS

## Цель

Установить Claude Code и Free Claude Code, настроить подключение к модели через OpenRouter и проверить ответ в терминале.

## Что сделано

1. На Mac установлены Claude Code и сторонний инструмент Free Claude Code.
2. В OpenRouter создан API-ключ; в настройках Free Claude Code выбран провайдер OpenRouter. Ключ в репозиторий не добавлен.
3. В настройках указана бесплатная модель NVIDIA Nemotron 3 Ultra через OpenRouter.
4. Claude Code запущен из отдельной папки. На тестовый вопрос получен ответ.
5. В статистике OpenRouter отображались запросы и расходы $0.00 за выбранный период; в разделе статистики показана модель Nemotron 3 Ultra.
6. В Claude Code подключены два MCP-сервера: `time` для времени и часовых поясов и `fetch` для чтения веб-страниц. Оба проверены в действии: получено время Бишкека и прочитана страница example.com.

## Скриншоты

- [Окно терминала с запуском и ответом](screenshots/terminal-window.png)
- [Настройка модели на платформе Free Claude Code](screenshots/platform-model-config.png)
- [Модель NVIDIA в OpenRouter](screenshots/openrouter-nvidia.png)
- [Активность OpenRouter и модель](screenshots/openrouter-activity.png)
- [Подключённые MCP-серверы](screenshots/mcp-connected.png)
- [Проверка обоих MCP-серверов](screenshots/mcp-tests.png)
- [Проверка ответа крупным планом](screenshots/terminal-test.png)
- [Карточка модели NVIDIA в OpenRouter](screenshots/nvidia-model.png)

Скрывайте API-ключи и личные данные перед публикацией. Снимок модели показывает часть страницы OpenRouter; если преподаватель требует всё окно, потребуется дополнительный снимок.

## Важно о провайдере

NVIDIA NIM и OpenRouter — разные провайдеры. Здесь используется модель NVIDIA через OpenRouter; прямое подключение к NVIDIA NIM не настроено, поскольку не удалось завершить проверку номера. Free Claude Code — сторонний проект, не официальный продукт Anthropic.

Для работы использованы два готовых MCP-сервера; собственный сервер не создавался. Их подключение выполнено в отдельной учебной папке Claude Code.
