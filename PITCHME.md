#HSLIDE

### HTML/CSS

![HTML5/CSS3](images/HTML-CSS3.jpg)

Сергей Денисов  
Старший фронтенд-разработчик

04.12.2017

#HSLIDE

### Библиотеки компонентов

* Основная цель: стандартизация компонентов на сайте и ускорение/упрощение разработки.
* Обычно состоят из: модульной сетки, компонентов, вспомогательных утилит и т.д.
* Обычно используют CSS-препроцессоры. 

Примеры:
* <a href="https://getbootstrap.com" target="_blank">Twitter Bootstrap</a> (<a href="https://jsfiddle.net/sergdenisov/hngh2bec/" target="_blank">использование</a>).
* <a href="http://hhru.github.io/bloko/" target="_blank">Bloko</a>.

#HSLIDE

### CSS: <a href="http://htmlbook.ru/content/modulnaya-setka" target="_blank">модульные сетки</a>.

<a href="http://htmlbook.ru/content/modulnaya-setka" target="_blank">Модульная сетка</a> представляет собой набор невидимых направляющих, вдоль которых
располагаются элементы страницы. Профит:

* Это облегчает размещение данных в документе.
* Обеспечивает визуальную связь между отдельными блоками.
* Сохраняет преемственность дизайна при переходе от одной страницы к другой.

#VSLIDE

Обычно состоит из:

* Контейнера.
* Строки.
* Ячейки.
* Отступов.

#VSLIDE

![CSS: Grid](images/grid.jpg)


Примеры: <a href="https://getbootstrap.com/docs/4.0/layout/grid/" target="_blank">Twitter Bootstrap</a>, <a href="http://960.gs" target="_blank">960 Grid System</a>.

#VSLIDE

### CSS: <a href="https://getbootstrap.com/docs/4.0/layout/grid/" target="_blank">модульная сетка в Twitter Bootstrap</a>

```html
<div class="container">
    <div class="row">
        <div class="col">
            One of three columns
        </div>
        <div class="col">
            One of three columns
        </div>
        <div class="col">
            One of three columns
        </div>
    </div>
</div>
```

#VSLIDE

### CSS: <a href="https://www.sitepoint.com/introduction-mobile-first-media-queries/" target="_blank">Mobile First</a>

![CSS: Mobile First](images/mobile-first.png)

Примеры: <a href="https://jsfiddle.net/sergdenisov/9mgrw25e/" target="_blank">Desktop First</a> vs <a href="https://jsfiddle.net/sergdenisov/8r8z3akx/" target="_blank">Mobile First</a>.

#HSLIDE

### CSS: <a href="https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Using_CSS_flexible_boxes" target="_blank">flexbox</a>

![CSS: flexbox](images/flexbox.png)

<a href="https://jsfiddle.net/sergdenisov/zwrroac2/" target="_blank">Пример 1</a>, <a href="https://jsfiddle.net/sergdenisov/95y31w8j/" target="_blank">пример 2</a>, <a href="http://frontender.info/a-guide-to-flexbox/" target="_blank">статья</a>.

#VSLIDE

Свойства flex-контейнера (родительского элемента):

```css
display: flex | inline-flex
flex-direction: row | row-reverse | column | column-reverse
flex-wrap: nowrap | wrap | wrap-reverse
flex-flow: <'flex-direction'> || <'flex-wrap'>
```

#VSLIDE

```css
justify-content: flex-start | flex-end | center |
                 space-between | space-around
```

![CSS: flexbox justify-content](images/justify-content.png)

#VSLIDE

```css
align-items: flex-start | flex-end | center |
             baseline | stretch
```

![CSS: flexbox align-items](images/align-items.png)

#VSLIDE

```css
align-content: flex-start | flex-end | center |
               space-between | space-around | stretch
```

![CSS: flexbox align-items](images/align-content.png)

#VSLIDE

Свойства дочерних элементов:

```css
order: <integer>
flex-grow: <number> (default 0)
flex-shrink: <number> (default 1)
flex-basis: <length> | auto (default auto)
flex: [<'flex-grow'> <'flex-shrink'>? || <'flex-basis'>]
      (default 0 1 auto)
align-self: auto | flex-start | flex-end | center |
            baseline | stretch
```

#HSLIDE

### CSS: <a href="https://www.urbaninsight.com/2012/04/12/ten-reasons-you-should-be-using-css-preprocessor" target="_blank">препроцессоры</a>

<a href="https://habrahabr.ru/sandbox/78148/" target="_blank">Препроцессоры</a> компилируют СSS код, который мы пишем на процессорном языке в чистый, валидный CSS код. Профит:

* Расширяют синтаксис CSS недостающими возможностями.
* Уменьшают дублирование кода.
* Делают код более структурированным.
* Упрощают поддержку кода.

#VSLIDE

### CSS: <a href="https://www.sitepoint.com/6-current-options-css-preprocessors/" target="_blank">популярные препроцессоры</a>

![CSS: preprocessors](images/preprocessors.jpg)

* <a href="http://sass-lang.com/guide" target="_blank">SASS/SCSS</a>.
* <a href="http://stylus-lang.com" target="_blank">Stylus</a>.
* <a href="http://lesscss.org/features/#features-overview-feature" target="_blank">LESS</a>.

#HSLIDE

### <a href="http://lesscss.org" target="_blank">LESS</a>

![LESS](images/less.jpg)

#VSLIDE

### LESS: <a href="http://lesscss.org/#using-less" target="_blank">использование</a>

* <a href="http://lesscss.org/#client-side-usage" target="_blank">Подключение скрипта</a>:

```html
<script src="less.js"></script>
```

* <a href="http://lesscss.org/#using-less-command-line-usage" target="_blank">Через командную строку</a>:

```bash
npm install -g less
 lessc styles.less
```

* <a href="https://www.npmjs.com/package/gulp-less" target="_blank">Через плагин для сборщика</a>.

#VSLIDE

### LESS: <a href="http://lesscss.org/features/#features-overview-feature-variables" target="_blank">переменные</a>

```less
@nice-blue: #5b83ad;
#header {
    color: @nice-blue;
}
```

```css
#header {
    color: #5b83ad;
}
```

#VSLIDE

### LESS: <a href="http://lesscss.org/features/#features-overview-feature-mixins" target="_blank">миксины</a>

```less
.my-mixin {
    color: black;
}
.my-other-mixin() {
    background: white;
}
.block {
    .my-mixin;
    .my-other-mixin;
}
```

```css
.my-mixin {
    color: black;
}
.block {
    color: black;
    background: white;
}

```

#VSLIDE

### LESS: <a href="http://lesscss.org/features/#mixins-parametric-feature" target="_blank">параметризированные миксины</a>

```less
.border-radius(@radius: 5px) {
    -webkit-border-radius: @radius;
    border-radius: @radius;
}
.button {
    .border-radius(6px);
}
```

```css
.button {
    -webkit-border-radius: 6px;
    border-radius: 6px;
}
```

#VSLIDE

### LESS: <a href="http://lesscss.org/features/#features-overview-feature-nested-rules" target="_blank">вложенные правила</a>

```less
#header {
    color: black;
    .navigation {
        font-size: 12px;
    }
    .logo {
        width: 300px;
    }
}
```

```css
#header {
    color: black;
}
#header .navigation {
    font-size: 12px;
}
#header .logo {
    width: 300px;
}

```

#VSLIDE

### LESS: <a href="http://lesscss.org/features/#features-overview-feature-nested-directives-and-bubbling" target="_blank">вложенные директивы и всплытие</a>

```less
.screen-color {
    @media screen {
        color: green;
        @media (min-width: 768px) {
            color: red;
        }
    }
    @media tv {
        color: black;
    }
}
```

#VSLIDE

### LESS: <a href="http://lesscss.org/features/#parent-selectors-feature" target="_blank">родительские селекторы</a>

```less
a {
    color: blue;
    &:hover {
        color: green;
    }
}
```

```css
a {
    color: blue;
}
a:hover {
    color: green;
}
```

#VSLIDE

### LESS: <a href="http://lesscss.org/features/#features-overview-feature-operations" target="_blank">математические операции</a>

```less
// numbers are converted into the same units
@conversion-1: 5cm + 10mm; // result is 6cm
@conversion-2: 2 - 3cm - 5mm; // result is -1.5cm
// conversion is impossible
@incompatible-units: 2 + 5px - 3cm; // result is 4px
// example with variables
@base: 5%;
@filler: @base * 2; // result is 10%
@other: @base + @filler; // result is 15%
```

```less
@base: 2cm * 3mm; // result is 6cm
```

```less
@color: #224488 / 2; // results in #112244
background-color: #112244 + #111; // result is #223355
```

#VSLIDE

### LESS: <a href="http://lesscss.org/features/#features-overview-feature-functions" target="_blank">функции</a>

```less
@base: #f04615;
@width: 0.5;
.class {
    width: percentage(@width); // returns 50%
    color: darken(@base, 5%); // returns #dd3d0e
    background-color: lighten(@base, 10%); // returns #f36c45
}
```

#VSLIDE

### LESS: <a href="http://lesscss.org/features/#loops-feature" target="_blank">циклы</a>

```less
.loop(@counter) when (@counter > 0) {
    .loop((@counter - 1)); // next iteration
    width: (10px * @counter); // code for each iteration
}
div {
    .loop(5); // launch the loop
}
```

```css
div {
    width: 10px;
    width: 20px;
    width: 30px;
    width: 40px;
    width: 50px;
}
```

#VSLIDE

### LESS: <a href="http://lesscss.org/features/#import-directives-feature" target="_blank">импорты</a>

```less
@import "foo"; // foo.less is imported
@import "foo.less"; // foo.less is imported
@import "foo.php";  // foo.php imported as a less file
@import "foo.css";  // statement left in place, as-is
@import (optional, reference) "foo.less";
@import (less) "foo.css";
```

#VSLIDE

### LESS: <a href="http://lesscss.org/features/#features-overview-feature-comments" target="_blank">комментарии</a>

```less
/* One hell of a block
style comment! */
@var: red;
// Get in line!
@var: white;
```

#HSLIDE

### Использование LESS в HeadHunter

* <a href="http://lesscss.org/features/#parent-selectors-feature" target="_blank">Родительские селекторы</a> только для элементов, модификаторов, псевдо-классов и псевдо-элементов.
* <a href="http://lesscss.org/features/#parent-selectors-feature" target="_blank">Родительские селекторы</a> ограничены 2-мя уровнями.
* Миксины только <a href="http://lesscss.org/features/#mixins-feature-not-outputting-the-mixin" target="_blank">со скобками</a> (чтобы не было в выходном файле).
* Не используются: <a href="http://lesscss.org/features/#extend-feature" target="_blank">Extend</a>, <a href="http://lesscss.org/features/#mixins-as-functions-feature" target="_blank">Mixins as Functions</a>, <a href="http://lesscss.org/features/#import-options" target="_blank">Import Options</a>.

#HSLIDE

### CSS: <a href="http://sixrevisions.com/css/css-methodologies/" target="_blank">методологии</a>

<a href="http://sixrevisions.com/css/css-methodologies/" target="_blank">CSS-методология</a> — способ написания и организации CSS-кода для упрощения поддержки и масштабирования проекта.

* <a href="http://oocss.org" target="_blank">Object-Oriented CSS (OOCSS)</a>
* <a href="https://smacss.com" target="_blank">Scalable and Modular Architecture for CSS (SMACSS)</a>
* <a href="https://ru.bem.info/methodology/quick-start/" target="_blank">Block, Element, Modifier (BEM)</a>

Полезное: <a href="https://habrahabr.ru/post/256109/" target="_blank">статья на Хабре</a>, <a href="http://getbem.com" target="_blank">альтернативный сайт про BEM</a>.

#HSLIDE

### <a href="https://ru.bem.info/methodology/quick-start/" target="_blank">Блок Элемент Модификатор</a>

![BEM](images/cap-bem.png)

#VSLIDE

### <a href="https://ru.bem.info/methodology/key-concepts/#Блок" target="_blank">БЭМ: блок</a>

![BEM: Block](images/block.png)

#VSLIDE

### <a href="https://ru.bem.info/methodology/key-concepts/#Свободное-перемещение" target="_blank">БЭМ: свободное перемещение блоков</a>

![BEM: Block moving](images/block-moving.png)

#VSLIDE

### <a href="https://ru.bem.info/methodology/key-concepts/#Повторное-использование" target="_blank">БЭМ: повторное использование блоков</a>

![BEM: Block using](images/block-using.png)

#VSLIDE

### <a href="https://ru.bem.info/methodology/key-concepts/#Элемент" target="_blank">БЭМ: элемент</a>

![BEM: Element](images/element.png)

#VSLIDE

### <a href="https://ru.bem.info/methodology/key-concepts/#Модификатор" target="_blank">БЭМ: модификатор</a>

![BEM: Modifier](images/modifier.png)

#HSLIDE

### <a href="https://ru.bem.info/methodology/naming-convention/#Соглашение-по-именованию" target="_blank">БЭМ: именование</a>

* БЭМ-сущностями называются блоки, элементы и модификаторы.
* Имена БЭМ-сущностей записываются с помощью цифр и латинских букв в нижнем регистре.
* Для разделения слов в именах используется дефис (-).
* Для хранения информации об именах блоков, элементов и модификаторов используются CSS-классы.

#VSLIDE

### <a href="https://ru.bem.info/methodology/naming-convention/#Имя-блока" target="_blank">БЭМ: имя блока</a>

```css
.block {
    ...
}
```

```html
<div class="block">...</div>
```

#VSLIDE

### <a href="https://ru.bem.info/methodology/naming-convention/#Имя-элемента" target="_blank">БЭМ: имя элемента</a>

```css
.block__element {
    ...
}
```

```html
<div class="block">
    <div class="block__element">...</div>
</div>
```

#VSLIDE

### <a href="https://ru.bem.info/methodology/naming-convention/#Имя-модификатора-блока" target="_blank">БЭМ: имя модификатора</a>

```css
.block_modifier {
    ...
}
.block_modifier-key_modifier-value {
    ...
}
```

```html
<div class="block block_modifier">
    ...
</div>
<div class="block block_modifier-key_modifier-value">
    ...
</div>
```

#VSLIDE

### <a href="https://ru.bem.info/methodology/naming-convention/#Имя-модификатора-элемента" target="_blank">БЭМ: имя модификатора элемента</a>

```css
.block__element_modifier {
    ...
}
.block__element__modifier-key_modifier-value {
    ...
}
```

```html
<div class="block">
    <div class="block__element block__element_modifier">
        ...
    </div>
</div>
<div class="block">
    <div class="block__element block__element_modifier-key_modifier-value">
        ...
    </div>
</div>
```

#VSLIDE

### <a href="https://ru.bem.info/methodology/naming-convention/" target="_blank">БЭМ: пример использования наименований</a>

```css
.form {}
.form_theme_forest {}
.form_login {}
.form__input {}
.form__submit {}
.form__submit_disabled {}
```

```html
<form class="form form_login form_theme_forest">
    <input class="form__input">
    <input class="form__submit form__submit_disabled">
</form>
```

#VSLIDE

### <a href="https://ru.bem.info/methodology/key-concepts/#Микс" target="_blank">БЭМ: миксы</a>

Микс — способ использования разных <a href="https://ru.bem.info/methodology/key-concepts/#БЭМ-сущность" target="_blank">БЭМ-сущностей</a> на одном элементе. Миксы позволяют:

* Совмещать поведение и стили нескольких БЭМ-сущностей без дублирования кода.
* Создавать семантически новые компоненты интерфейса на основе имеющихся БЭМ-сущностей.

```html
<div class="menu">
    <span class="menu__item link">...</span>
</div>
```

#HSLIDE

### CSS-методология в HeadHunter

"У нас свой подход, лишь отдалённо напоминающий БЭМ." (c):

* Есть глобальный `_defaults.less` (нормализация различных стилей браузеров по умолчанию).
* Миксы запрещены.
* Модификаторы только булевы.
* Иногда используются глобальные классы.
* Иногда используются глобальные модификаторы.
