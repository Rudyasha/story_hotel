# Story Hotel · QA

QA-документация по монетизации и механике ивента «Ключи / Открыть все». Оформление продолжает стиль [Todo](https://rudyasha.github.io/to_do_tz/) и [разбора инцидента](https://rudyasha.github.io/incident/): Material for MkDocs, русский поиск, светлая и тёмная темы.

**Сайт:** [Story Hotel · QA](https://rudyasha.github.io/story_hotel/)

## Разделы

| Раздел | Содержание |
| --- | --- |
| [01 · Чек-листы по монетизации](docs/index.md) | Магазин, покупки, акции, наборы, обмен валют, реклама и backend |
| [02 · Вопросы к аналитику](docs/analyst-questions.md) | 23 вопроса: экономика, поле, награды, оплата и восстановление |
| [03 · Тест-кейсы по функционалу](docs/test-cases.md) | 5 кейсов с предусловиями, шагами и ожидаемыми результатами |
| [04 · Баг-репорты](docs/bug-reports.md) | Шаблон отчёта и форма GitHub Issues для найденных дефектов |

Материалы подготовлены по предоставленному тексту. Прогоны игры не проводились; спорные правила вынесены в вопросы и допущения. Подтверждённые дефекты не предоставлены.

## Локальный просмотр

```sh
python3 -m venv .venv
.venv/bin/pip install -r requirements.txt
.venv/bin/mkdocs serve
```

Проверка сборки: `.venv/bin/mkdocs build --strict`.

## Редактирование и публикация

Тексты - в `docs/`, навигация - в `mkdocs.yml`, стили - в `docs/assets/styles.css`. Форма нового дефекта - в `.github/ISSUE_TEMPLATE/bug-report.yml`.

GitHub Actions собирает и публикует документацию после push в `main`. Источник публикации в **Settings → Pages** - **GitHub Actions**.
