# MeetSpace — макеты для смартфона и планшета

Интерактивный дизайн-прототип MeetSpace на HTML, CSS и JavaScript. Галерея показывает интерфейс смартфона и планшета, поддерживает светлую и тёмную темы и поворот планшета.

## Локальный запуск

Из корня репозитория выполните:

```sh
python3 meetspace-refresh-20261016/serve.py 8766
```

Откройте [галерею макетов](http://127.0.0.1:8766/index.html). Для просмотра не нужны сборка, npm-зависимости или подключение к серверу MeetSpace. Для демонстрационного входа используйте пароль `demo`.

[Установщик: смартфон и планшет](http://127.0.0.1:8766/index.html?screen=deploy&view=compare&theme=light&v=20261114-installer-parity).

Прямые ссылки на настройки:

- [Профиль](http://127.0.0.1:8766/index.html?screen=settings&section=profile&view=compare&theme=light).
- [Аудио](http://127.0.0.1:8766/index.html?screen=settings&section=audio&view=compare&theme=light).
- [Видео](http://127.0.0.1:8766/index.html?screen=settings&section=video&view=compare&theme=light).
- [Уведомления](http://127.0.0.1:8766/index.html?screen=settings&section=notifications&view=compare&theme=light).

## Содержимое

- [`meetspace-refresh-20261016/index.html`](meetspace-refresh-20261016/index.html) — галерея экранов и сравнение устройств.
- [`meetspace-refresh-20261016/preview.html`](meetspace-refresh-20261016/preview.html) — отдельный экран прототипа.
- [`meetspace-refresh-20261016/handoff.html`](meetspace-refresh-20261016/handoff.html) — описание дизайна, сценариев и ограничений.
- [`meetspace-refresh-20261016/installer-parity.md`](meetspace-refresh-20261016/installer-parity.md) — соответствие установщику Android: экраны, диагностика, восстановление и границы проверенного UI-прототипа.
- `meetspace-refresh-20261016/assets/` — локальные шрифты, иконки и демонстрационные материалы.
- `meetspace-refresh-20261016/previews/` и PNG-файлы в корне — снимки экранов разных этапов разработки.
- `qa-*.json`, `qa-report.json`, `regression-report.json` и `verify.mjs` — исторические отчёты и сценарий браузерной проверки. Для запуска сценария отдельно нужен Playwright; отчёты относятся к состоянию макета на дату их создания.

## Возможности макета

Встречи и видеовстречи, личные и групповые чаты, действия с сообщениями, папки, записи, уведомления, несколько аккаунтов, настройки аудио и видео, редактирование аватарок пользователя и группы.

Все данные демонстрационные. Звонки, доступ к камере и микрофону, операции с аккаунтами и отправка уведомлений имитируются. Состояние интерфейса хранится в памяти до перезагрузки страницы.
