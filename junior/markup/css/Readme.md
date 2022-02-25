# Секция CSS

> Что такое CSS?
> 
[link](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps)

> Как работает CSS?
>
[link](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_works)

> Как можно применить стили CSS к HTML разметке? Плюсы и минусы каждого подхода
>
[link](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_is_structured)

## Фундамент CSS
> Что такое каскадность в CSS?

> Что такое специфичность в CSS, как считается?

> Как работает наследование в CSS

[link](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Cascade_and_inheritance)

## Единицы измерения в CSS
> Назовите основные единицы измерения в CSS

> В чем отличие rem от em, когда удобно использовать эти единицы
[link](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Values_and_units#lengths)

## CSS Box model

> Что такое box model в CSS?

> В чем отличие padding от margin?

> Как рассчитывается высота и ширина элемента со свойством `box-sizing: border-box;`

[link](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model#what_is_the_css_box_model)

## Адаптивность
> За счет чего достигается адаптивность сайтов?

> Напишите media запрос для планшетов (от 768px до 992px включительно)

[link](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)

## CSS Layout

### Позиционирование

> Назовите основные значения свойства `position`

> Что такое normal flow и out of flow?

> Как позиционируется элемент со свойством `position: absolute;`?

[Позиционирование](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Positioning)

[Normal flow](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Normal_Flow)

### Flexbox

> Назовите основные свойства flexbox layout относящиеся к flex-контейнеру

> Назовите основные свойства flexbox layout относящиеся к flex-элементу

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
    <style>
        .container {
            width: 400px;
            height: 400px;
            background-color: deepskyblue;

            display: flex;
            flex-direction: column;
            justify-content: end;
            align-items: flex-start;
        }

        .element {
            width: 50px;
            height: 50px;
            background-color: yellow;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="element"></div>
    </div>
</body>
</html>
```
> Выше дана страница. В каком углу будет находится элемент относительно контейнера?

[Flexbox](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox)

[Flexbox cheat sheet](https://flexbox.malven.co/)

### Grids

> В чем суть Grid layout?

> Как работают функции minmax, repeat?

[Grids](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Grids)

[Grids cheat sheet](https://grid.malven.co/)

## Препроцессоры SASS/LESS*

> Назовите плюсы использования препроцессоров

> Для чего используются функции `@include, @mixin, @function`

[link](https://sass-lang.com/guide)


## Методологии*

> Объясните суть методолгии BEM

[link](https://ru.bem.info/methodology/quick-start/)

*Методолгий много, по опыту БЭМ самая распространненая*
