# Начало работы

Для установки рекомендуется использовать [Yeoman](http://yeoman.io/):

```bash
npm install -g yo
```

После yeoman, необходимо установить шаблон самой сборки:

```bash
npm install -g generator-ninelines-template
```

Теперь находясь в пустой папке с проектом выполняем команду:

```bash
yo ninelines-template
```

Генератор задаст несколько вопросов:

- Название проекта (по умолчанию — название папки проекта).
- Описание проекта.
- Запустить ли `npm install` (по умолчанию — да). Если пропустить установку npm-пакетов, то перед началом работы над проектом необходимо самостоятельно запустить `npm install`.

Теперь можно запустить `gulp` и приступить к работе.