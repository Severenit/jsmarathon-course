# Homework #2

За этот урок мы узнали много маленьких, но очень важных вещей.

И пора их всех применить на практике.

Мы должны освоить пройденный материал, закрепить использование библиотеки [classNames](https://www.npmjs.com/package/classnames), [propTypes](https://ru.reactjs.org/docs/typechecking-with-proptypes.html) и передачи **props** в компоненты.

## Компонент <Header />

Давайте чуть исправим заголовок, прежде всего возьмите текущий код для стилей компонента `<Header />`

```css
.root {
    height: 80px;
}

.headerWrap {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.header {
    height: 80px;
    width: 100%;
    transition: height 0.2s linear, box-shadow 0.2s linear;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 100;
    background: rgba(245, 245, 245, 0.97);
    display: flex;
    justify-content: center;
    align-items: center;
}

.header.small {
    height: 60px;
    box-shadow: 0px 1px 3px 0px rgba(50, 50, 50, 0.8);
}

.logo {
    height: 70px;
    width: 125px;
}

.nav {
    display: flex;
    list-style: none;
    margin: 0;
    padding: 0;
    font-size: 18px;
    transition: font-size 0.2s linear;
}

.nav li {
    position: relative;
}

.nav li a {
    transition: color 0.2s linear;
}

.nav li:hover a {
    color: red;
}

.nav li a {
    padding: 21px;
    color: initial;
    text-decoration: initial;
}

.header.small .logo {
    width: 89px;
    height: 50px;
}

.header.small .nav  {
    font-size: 16px;
}
```

В наш **div** с классом .logo вставим картинку логотипа.

Картинку вы можете скачать отсюда [logo.png](https://firebasestorage.googleapis.com/v0/b/it-course-84ddd.appspot.com/o/course%2Freact%2F02%2Flogo.png?alt=media&token=5cda9c00-1d3c-431f-9f3a-d6bff9022842)

UPD: Нашему контейнеру которое оборачивает logo и menu дадим класс **.headerWrap**

## Компонент <Container />

Конечно, чаще всего такой компонент называется *Layout*. И такие компоненты существуют почти в каждом React приложение. Этот компонент имеет единую обертку над контентом.

Мы уже с вами создали его в уроке, так что вам просто его нужно повторить и применить в нужном месте.

Не забывайте о **propTypes**

## Компонент <Heading />

В целом мы создали этот компонент в уроках.

Но давайте теперь сделаем стили для ***пяти*** типов заголовков, больше использовать не будем.

Для заголовка первого `h1` типа:

```css
margin-bottom: 0.5em;
color: #000000d9;
font-weight: 600;
font-size: 38px;
line-height: 1.23;
```

Для заголовка второго `h2` типа:

```css
margin-bottom: 0.5em;
color: #000000d9;
font-weight: 600;
font-size: 30px;
line-height: 1.35;
```

Для заголовка третьего `h3` типа:

```css
margin-bottom: 0.5em;
color: #000000d9;
font-weight: 600;
font-size: 24px;
line-height: 1.35;
```

Для заголовка четвертого `h4` типа:

```css
margin-bottom: 0.5em;
color: #000000d9;
font-weight: 600;
font-size: 20px;
line-height: 1.4;
```

Для заголовка пятого `h5` типа:

```css
margin-bottom: 0.5em;
color: #000000d9;
font-weight: 600;
font-size: 16px;
line-height: 1.5;
```

Посмотрите какие вещи можно вынести в класс `.root`, а какие присвоить только определенным типам.

Не забудьте для всех заголовков сбросить **margin** и **padding**

## Компонент <Text />

А теперь давайте создадим “умный” 😝 компонент (этот компонент не имеет ничего общего с настоящим понятием что такое умный и глупый компонент. *примечание автора*)

Компонент `<Text />` должен включать в себя несколько **props**

- **element** - он может быть одним из элементов `div` `p` `span`
- **children** - то что мы передадим как дочерние узлы
- **className** - мы всегда должны иметь возможность добавить дополнительные классы нашему компоненту
- **strong** - это boolean переменная делает текст внутри компонента либо жирным либо нет
- **italic** - это boolean переменная делает текст внутри компонента либо курсивом либо нет
- **disabled** - делает наш текст внутри компонента недоступным, добавляет прозрачности в 0.6, а так же добавляет `cursor: not-allowed;`

Все эти компоненты расположите в новом блоке между `<Slider />` и `<Footer />`

У рутового компонента который вы расположите по аналогии со Slider задайте цвет фона `background: #f7f7f7;`

Так же сделайте скриншот получившегося результата. И прикрепите его в описание к PR (pull request)

## 02.09 - Как создать PR (pull request)

[$embed](https://vimeo.com/698292175)

Желаю удачи...

Ссылку на PR жду в окне ниже
