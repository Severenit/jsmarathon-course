# Homework #6

По мимо того что вам надо сделать тоже что и в уроках. Вам нужно сделать две вещи.

## #1 ScrollTop

![HM6](https://firebasestorage.googleapis.com/v0/b/it-course-84ddd.appspot.com/o/course%2Freact%2F06%2FHM6-2.gif?alt=media&token=b6baee33-6719-4686-add0-f383dca53a1f)

Посмотрите внимательно на видео выше. Вы увидите что при переключении между страниц наша страница всегда остается на том положении что мы были на предедущей. А надо всегда подниать страницу наверх.

В этом вам поможет `useEffect` который в зависимостях будет следить за изменениями в `location.pathname`

## #2 Создадим Anchor Link

![HM6-2](https://firebasestorage.googleapis.com/v0/b/it-course-84ddd.appspot.com/o/course%2Freact%2F06%2FHM6.gif?alt=media&token=b1383de1-f3d2-46ef-894d-5d3ca7fb5838)

Посмотрите на видео выше и вы увидите что теперь мы должны создать рядом с заголовком иконку, нажимая на которую мы добавляем к нашему url якорную ссылку.

Теперь если мы скопируем ее и вставим в другую вкладку нас должно проскролить к ней.

Здесь вам может помочь метод у элемента `scrollIntoView`

```js
element.scrollIntoView({
    block: 'center',
    behavior: 'smooth'
});
```

Ну а так же вам может потребоваться эта иконка [SVG Icon](https://firebasestorage.googleapis.com/v0/b/it-course-84ddd.appspot.com/o/course%2Freact%2F06%2Flink_icon.svg?alt=media&token=5e6ab9c1-29b9-4e18-820c-f9c1eed07a14)

Не забывайте обращаться за помощью к своим товарищам, кураторам и гуглу...

Ну а на этом все, жду ваши PR, до встречи очень скоро...

Let's keep in touch!
