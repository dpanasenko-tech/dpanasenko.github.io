# dpanasenko-tech.github.io

Персональный био-лендинг Дениса Панасенко — <https://dpanasenko-tech.github.io/>

Статический сайт без сборки: GitHub Pages отдаёт файлы из ветки `main` как есть.
Файл `.nojekyll` отключает обработку Jekyll, поэтому push сразу попадает в эфир.

## Структура

    index.html            RU-версия (главная)
    en/index.html         EN-версия
    assets/css/style.css  единственный стилевой файл
    assets/img/me.jpg     фото для hero-блока
    .nojekyll             отключает сборку Jekyll

## Локальный просмотр

    python3 -m http.server 8080

Затем открыть <http://localhost:8080/>. Обычный `open index.html` не подойдёт:
пути к CSS и картинке абсолютные (`/assets/...`) и требуют HTTP-сервера.

## Правки

Тексты живут прямо в HTML. Любое изменение смысла нужно вносить в обе версии —
`index.html` и `en/index.html`.
