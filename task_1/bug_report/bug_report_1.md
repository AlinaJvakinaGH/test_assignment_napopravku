
# Несоответствие верстки с макетом дизайна (отсутствие точности до "пиксель-перфект" в поп-ап)

В мобильной и десктопной версии границы поп-ап в профиле для заполнения информации о пациенте на Chrome, Яндекс, Mozilla Firefox, отображается не так, как на макете в фигме.

### Шаги воспроизведения на десктоп версии

1. Перейти по [ссылке](http://landing.hh-demo.np-internal.ru/) в одном из трёх браузеров (Chrome, Яндекс, Mozilla Firefox);
2. Нажать на кнопку “Перейти к заполнению” в блоке;
3. Открыть DevTools, выставить формат экрана как у макета в фигме для десктоп версии (1919/1314);
4. Сравнить отображение элементов страницы с макетом в Figma с использованием инструмента Pixel Perfect Pro или аналогами.

### Шаги воспроизведения на мобильной версии

1. Перейти по [ссылке](http://landing.hh-demo.np-internal.ru/) в одном из трёх браузеров (Chrome, Яндекс, Mozilla Firefox);
2. Нажать на кнопку “Перейти к заполнению” в блоке;
3. Открыть DevTools, выставить формат экрана как у макета в фигме для мобильной версии (375/1589);
4. Сравнить отображение элементов страницы с макетом в Figma с использованием инструмента Pixel Perfect Pro или аналогами.

### Текущий результат десктоп и мобильной версий

**Десктоп версия:**

- указана верхняя внутренняя граница блока и нулевое значение верхней внешней границы (padding-top: 32px, margin-top: 0px);
- указаны margin-left и margin-right со значением 281.5px;
- нет свойства border-radius для скругления углов поп-апа со значением 8px.

**Mozilla Firefox:**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfv3TdcqteFDMeKr_aFOoA9HcG7EGfyqMjpD0WVkwxBCBn71hhjpFYckG3luGyMURLIar5Bx78c3fOlWDI6lcL4nHuLsl6IkGwSJ__vMsEinbG1Yr8o7Y4hYxfbLdnkkJ3D_okELN_OjE2kgvdqsK7r9CE?key=5zm4E5ppL1fPPahAzLazLw)

**Chrome:**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdt7tvOZDOPX61WdK5C-OmDAh_s3azHP0Iom4Jcgolp64rnFWRZGMO6oHAcfPOQbO9mzRzID7B46qbpgMfJzykU8w6wpofUp--z-jE6HlN6z-g6dGD9PGPquzYx3kOrHMyuFRkAMxWp2iCrb_wsdzUb7Iw?key=5zm4E5ppL1fPPahAzLazLw)

**Мобильная версия:**

- width: 588.033px;
- нет свойства height со значением 1589px
- нет свойства Top со значением 191px
- нет свойства left со значением -483px

**Mozilla Firefox**

[Скринкаст некорректной верстки](https://drive.google.com/file/d/18YrCRQgqjGnsXaN8duT5Oa_kd7_pATIS/view?usp=sharing)

**Яндекс**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXeiGxeftv5N-i7M5tJ8JwXfShE9ZW60UiQBjCnqOjIo4GCCcDg6qzVIwJ96CWUI2AtvFfAKJ0tzXODMZLD76YjFjzh7p8SXPejkKPY4dcSs5_E_oGpoysYec5b94a5TKRielJJfM-cVJ6OGCGDtQBFbUZA?key=5zm4E5ppL1fPPahAzLazLw)

### Ожидаемый результат десктоп и мобильной версии

Элементы страницы должны соответствовать макету:

[Ссылка на макет в фигме](https://www.figma.com/design/Y4bDSYRs6RcQOUstBjgzlH/%D0%9D%D0%B0%D0%9F%D0%BE%D0%BF%D1%80%D0%B0%D0%B2%D0%BA%D1%83---%D1%82%D0%B5%D1%81%D1%82%D0%BE%D0%B2%D0%BE%D0%B5-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-%D0%B4%D0%BB%D1%8F-%D0%B2%D0%B5%D1%80%D1%81%D1%82%D0%B0%D0%BB%D1%8C%D1%89%D0%B8%D0%BA%D0%B0?node-id=0-1&viewport=509%252C302%252C)

### Окружение

Браузеры:

- Chrome. Версия 125.0.6422.61
- Яндекс. Версия 122.0.6261.952
- Mozilla Firefox. Версия 125.0.2 (64arm)

### Тестовое устройство

- Ноутбук ASUSTeK COMPUTER INC X550VB. Версия 1.0
- OS Linux Mint 20

### Аналитика

Здесь должна быть ссылка на яндекс-метрику (или другую Вашу метрику) с количеством пользователей, которых задевает данная проблема.

### Серьёзность

- Minor
