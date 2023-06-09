# Структура папок и файлов

```text
ninelines-template
├── src
│   ├── images
│   │   └── sprites
│   │       ├── png
│   │       │   └── .keep
│   │       └── svg
│   │           └── .keep
│   ├── js
│   │   ├── vendor
│   │   │   └── .keep
│   │   ├── main.js
│   │   └── vendor.js
│   ├── pug
│   │   ├── mixins
│   │   │   └── svg.pug
│   │   ├── base.pug
│   │   └── mixins.pug
│   ├── resources
│   │   └── fonts
│   │       └── .keep
│   ├── scss
│   │   ├── functions
│   │   │   └── _sprites.scss
│   │   ├── mixins
│   │   │   ├── _clearfix.scss
│   │   │   ├── _retina.scss
│   │   │   ├── _sprites.scss
│   │   │   ├── _triangle.scss
│   │   │   └── _visually-hidden.scss
│   │   ├── vendor
│   │   │   └── .keep
│   │   ├── _base.scss
│   │   ├── _fonts.scss
│   │   ├── _functions.scss
│   │   ├── _mixins.scss
│   │   ├── _sprites.hbs
│   │   ├── _sprites.scss
│   │   ├── _variables.scss
│   │   ├── _vendor.scss
│   │   └── main.scss
│   └── index.pug
├── .babelrc
├── .editorconfig
├── .eslintignore
├── .eslintrc
├── .gitignore
├── .npmrc
├── .pug-lintrc.json
├── .stylelintignore
├── .stylelintrc
├── gulpfile.js
├── package.json
├── README.md
└── webpack.config.js
```

## `src`

В папке `src` хранятся исходные файлы проекта.

## `src/images`

Папка `images` предназначена для хранения изображений.
При сборке файлы из данной папки попадают в `build/images`.

## `src/images/sprites`

Папка `src/images/sprites` предназначена для хранения векторных (SVG) и растровых (PNG) иконок.

## `src/images/sprites/png`

Папка `src/images/sprites/png` предназначена для хранения растровых иконок.
При сборке файлы из данной папки объединяются в два спрайта: `build/images/sprites.png` и `build/images/sprites@2x.png`.

## `src/images/sprites/svg`

Папка `src/images/sprites/svg` предназначена для хранения векторных иконок.
При сборке файлы из данной папки объединяются в один спрайт: `build/images/sprites.svg`.

## `src/js`

Папка `src/js` предназначена для хранения скриптов.

## `src/js/vendor`

Папка `src/js/vendor` предназначена для хранения скриптов сторонних библиотек, которых нет в репозитории npm.

## `src/js/main.js`

Файл `src/js/main.js` предназначен для хранения основной логики сайта.
При сборке данный файл попадает в `build/js`.

## `src/js/vendor.js`

Файл `src/js/vendor.js` предназначен для подключения сторонних библиотек.

При сборке данный файл попадет в `build/js`.

## `src/pug`

Папка `src/pug` предназначена для хранения шаблонов.

## `src/pug/mixins`

Папка `src/pug/mixins` предназначена для хранения Pug-миксин.

## `src/pug/base.pug`

В файле `src/pug/base.pug` хранится базовый шаблон страниц сайта.

## `src/pug/mixins.pug`

Файл `src/pug/mixins.pug` предназначен для подключения Pug-миксин из папки `src/pug/mixins`.

## `src/resources`

Папка `src/resources` предназначена для хранения различных файлов проекта.
При сборке файлы из данной папки попадают в `build`.

## `src/resources/fonts`

Папка `src/resources/fonts` предназначена для хранения шрифтов.
При сборке файлы из данной папки попадают в `build/fonts`.

## `src/scss`

Папка `src/scss` предназначена для хранения стилей.

## `src/scss/functions`

Папка `src/scss/functions` предназначена для хранения SCSS-функций.

## `src/scss/mixins`

Папка `src/scss/mixins` предназначена для хранения SCSS-миксин.

## `src/scss/vendor`

Папка `src/scss/vendor` предназначена для хранения стилей сторонних библиотек, которых нет в репозитории npm.

## `src/scss/_base.scss`

Файл `src/scss/_base.scss` предназначен для хранения базовых стилей.

## `src/scss/_fonts.scss`

Файл `src/scss/_fonts.scss` предназначен для подключения шрифтов.

## `src/scss/_functions.scss`

Файл `src/scss/_functions.scss` предназначен для подключения функций из папки `src/scss/functions`.

## `src/scss/_mixins.scss`

Файл `src/scss/_mixins.scss` предназначен для подключения миксин из папки `src/scss/mixins`.

## `src/scss/_sprites.hbs`

`src/scss/_sprites.hbs` — шаблон, на основе которого генерируется содержимое файла `src/scss/_sprites.scss`.

## `src/scss/_sprites.scss`

Файл `src/scss/_sprites.scss` предназначен для работы с PNG-спрайтами.
Содержимое данного файла автоматически генерируется на основе шаблона `src/scss/_sprites.hbs` и иконок из папки `src/images/sprites/png`.

## `src/scss/_variables.scss`

Файл `src/scss/_variables.scss` предназначен для хранения SCSS-переменных.

## `src/scss/_vendor.scss`

Файл `src/scss/_vendor.scss` предназначен для подключения стилей сторонних библиотек.

## `src/scss/main.scss`

Файл `src/scss/main.scss` предназначен для хранения основных стилей сайта.
При сборке данный файл преобразуется в CSS и сохраняется в `build/css` вместе с файлом `main.css.map`.

## `src/index.pug`

`src/index.pug` — шаблон главной страницы.
При сборке все Pug-файлы из папки `src` преобразуются в HTML и сохраняются в `build`.

## `.babelrc`

`.babelrc` — файл настроек JavaScript-транспайлера Babel.

## `.editorconfig`

`.editorconfig` — файл настроек редактора.

## `.eslintignore`

`.eslintignore` — файл настроек ESLint для игнорирования файлов.

## `.eslintrc`

`.eslintrc` — файл настроек ESLint.

## `.gitignore`

`.gitignore` — файл настроек Git для игнорирования файлов.

## `.npmrc`

`.npmrc` — файл настроек npm.

## `.pug-lintrc.json`

`.pug-lintrc.json` — файл настроек pug-lint.

## `.stylelintignore`

`.stylelintignore` — файл настроек stylelint для игнорирования файлов.

## `.stylelintrc`

`.stylelintrc` — файл настроек stylelint.

## `gulpfile.js`

`gulpfile.js` — основной файл сборки, содержащий Gulp-задачи.

## `package.json`

`package.json` — файл, содержащий базовую информацию о проекте и список требуемых библиотек.

## `README.md`

`README.md` — описание проекта.

## `webpack.config.js`

`webpack.config.js` — файл настроек webpack.
