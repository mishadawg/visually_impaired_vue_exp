# visually_impaired_vue_exp
Пример использования библиотеки https://bvi.isvek.ru/ для vue 3.
Все настройки плагина https://github.com/veks/button-visually-impaired-javascript в разделе Settings.
В исходниках bvi.js уже пофикшена ошибка инициалазиции.
Стили плагина правятся в bvi.css.

Todo адаптировать плагин под реактивность vue/react.
Сейчас работа с изображением возможна только в том случае если плагин запущен и на той же странице можно работать с картинками
(скрывать изображения,обсцвечивать,оставлять без изменений).
При переходе на другую страницу,плагин не видит уже изображения(не прокидывает свои классы чтобы подвязаться к картинкам).

### Settings
Option | Type | Default value| Value options | Description
------ | ---- | ------- | -------------- | -----------
target | string |  '.bvi-open' | '.className' | Plugin initialization class |
fontSize | number |  16 | 1-39 | Font size  |
theme | string |  'white' |  (`white`&#124;`black`&#124;`blue`&#124;`brown`&#124;`green`) | Color spectrum |
images |(string&#124;boolean) | 'grayscale' |  (`true`&#124;`false`&#124;`grayscale`) | Adapting images |
letterSpacing | string | 'normal' | (`normal`&#124;`average`&#124;`big`) | Letter spacing |
lineHeight | string | 'normal' | (`normal`&#124;`average`&#124;`big`) | Line spacing |
speech | boolean | true | (`true`&#124;`false`) | Speech synthesis |
fontFamily | string | 'arial' |  (`arial`&#124;`times`) | Fonts |
builtElements | boolean | false | (`true`&#124;`false`) | Inline elements are a component of an HTML element that allows you to embed documents, videos, maps, and interactive media into a page.|
panelFixed | boolean | true | (`true`&#124;`false`) | Fixing the panel for the visually impaired at the top of the page. |
panelHide | boolean | false | (`true`&#124;`false`) | Hides the panel for the visually impaired and shows the panel icon. |
reload | boolean | false | (`true`&#124;`false`) | Enable / Disable page reload when switching to the regular version of the site. |
lang | string | 'ru-RU' | (`'ru-RU'`&#124;`'en-US')`| Language |

## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```