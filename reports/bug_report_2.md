
# Несоответствие верстки с макетом дизайна (отсутствие точности до "пиксель-перфект" на странице заполнения информации о пациенте в блоке с кнопкой, открывающей поп-ап)

В десктопной версии нижняя часть блока с кнопкой для перехода в поп-ап на Google Chrome, Яндекс, Mozilla Firefox, отображается не так, как на макете в фигме.

В мобильной версии границы главного блока отображаются не так, как в фигме.

### Шаги воспроизведения на десктоп версии

1. Перейти по [[ссылке](http://landing.hh-demo.np-internal.ru/)](http://landing.hh-demo.np-internal.ru/) в одном из трёх браузеров (Google Chrome, Яндекс, Mozilla Firefox);
2. Открыть DevTools, выставить формат экрана как у макета в фигме для десктопной версии (1919/1080);
3. Сравнить отображение элементов страницы с макетом в Figma с использованием инструмента Pixel Perfect Pro или аналогами.

### Шаги воспроизведения на мобильной версии

1. Перейти по [ссылке](http://landing.hh-demo.np-internal.ru/) в одном из трёх браузеров (Google Chrome, Яндекс, Mozilla Firefox);
2. Открыть DevTools, выставить формат экрана как у макета в фигме для мобильной версии (375/859);
3. Сравнить отображение элементов страницы с макетом в Figma с использованием инструмента Pixel Perfect Pro или аналогами.

### Текущий результат десктопной и мобильной версий

**десктоп версия**

- высота блока 653,017px;
- недостаточный отступ между изображением и текстом ниже.

**Google Chrome:**
![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdorYVhCPAUzLW0Y6zZFYisDxhf9L4n1gHirfqSs_T6iUM0VWbldPHQpK8NJCddgkAKoZSCUEZh9nauDQeXmswBlayUV6T9kg35yAaciO13i-HOnSG1-IfQFMvSeRMn6xaYoZgHmD31iK9CJbYGQCszJrU_?key=W9WZZmEcmfVJofTw_hOVLg)

**Mozilla Firefox:**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfzYiAZrHxA7lWvE3SwOi11DqDjH1WQFKFVkJUs-dcCvHoXVZNItfWaA1JNntqv48QUo5Uvl24K21X4CMfzfaDsIw8so2syPqKwo1DEeSZ1v2fr_seurXE6yVRpn71su5bdPppr3Gc6FbKL2j3wZqaHC8n4?key=W9WZZmEcmfVJofTw_hOVLg)

**Мобильная версия:**

- height: 614.438px
- width: 356px
- нет свойства Top со значением -1135px
- нет свойства left со значением -483px

**Яндекс**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXduIPQ4--535StqfDSIqz8nxewoV52LcqEQe8FY4__qMz8MBt1Gk3Cc4yos9puajnfQlv6KZ-8MUnGEZ3aDnO9uFZM0SZZtkfvGUcf3d5jXA7FzNR7UOJ8g9z0zrxuTegl4oXGEtp0EFhiNeGUmYt5KJd8?key=W9WZZmEcmfVJofTw_hOVLg)

**Google Chrome**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfQ9f_2YyLNVFer8BeKj99w9lmFF0DGLiU1T1IE7YUygEw5Pu5a5BTW4SaWD38HWjZz7I1nt5v9YIX4BkBpENu28SvET1FmmjZ7JgBPWvSBOhxvwMhJtVaoxaKV2bzDab5JGtnbyA5tkJsP_2QznM9M7wRI?key=W9WZZmEcmfVJofTw_hOVLg)

### Ожидаемый результат десктопной и мобильной версий

Элементы страницы должны соответствовать макету в Figma:

[Ссылка на макет в фигме](https://www.figma.com/design/Y4bDSYRs6RcQOUstBjgzlH/%D0%9D%D0%B0%D0%9F%D0%BE%D0%BF%D1%80%D0%B0%D0%B2%D0%BA%D1%83---%D1%82%D0%B5%D1%81%D1%82%D0%BE%D0%B2%D0%BE%D0%B5-%D0%B7%D0%B0%D0%B4%D0%B0%D0%BD%D0%B8%D0%B5-%D0%B4%D0%BB%D1%8F-%D0%B2%D0%B5%D1%80%D1%81%D1%82%D0%B0%D0%BB%D1%8C%D1%89%D0%B8%D0%BA%D0%B0?node-id=0-1&viewport=509%252C302%252C)

### Окружение

Браузеры:

- Google Chrome. Версия 125.0.6422.61
- Яндекс. Версия 122.0.6261.952
- Mozilla Firefox. Версия 125.0.2 (64arm)

### Тестовое устройство

- Ноутбук ASUSTeK COMPUTER INC X550VB. Версия 1.0
- OS Linux Mint 20

### Аналитика

Здесь должна быть ссылка на яндекс-метрику (или другую Вашу метрику) с количеством пользователей, которых задевает данная проблема.

### Приоритет

- Minor

### Серьёзность

- Trivial
