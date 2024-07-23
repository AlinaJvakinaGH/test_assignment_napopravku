# В поп-апе на странице заполнения профиля категории заболеваний под инпутом выходят за рамки блока при увеличении масштаба

При изменении масштаба с 100% до минимального разрешения экрана (320%) категории заболеваний под инпутом выходят за рамки поп-апа.

### Шаги воспроизведения на десктопной версии

1. Перейти по [ссылке](http://landing.hh-demo.np-internal.ru/) в одном из трёх браузеров (Chrome, Яндекс, Mozilla Firefox);
2. Изменить масштаб страницы со 100% до 320%

### Шаги воспроизведения на мобильной версии

1. На телефонне перейти по [ссылке](http://landing.hh-demo.np-internal.ru/) в одном из трёх браузеров (Chrome, Яндекс, Mozilla Firefox);
2. Сравнить вёрстку с макетом в фигме.

### Текущий результат

**десктоп версия**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfgkZEMoPIMVe_BX97fWsxbgjCrb9uLbcRAVIaeolxiuSXL_Infju_XgLVAdUXTae4uvugjJ2ADBJDgeMRxhqug-i2AlTsSgFRhRzRFvfmpnK2NoDZr_y93eR4eQrqNMdhfAP3UVsarOA9u-KU4CVi6JQmQ?key=2Yj3j6m_mrGSAHOLnVn3pg)

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXeYnSTmMlSEFbuBM4yFh7oggllma4pbO89IpPwu1l_4xV7CYbZfGj4y8iWhb89NEkhnQIUb7QjLDjXqJvuK02kKR2iwT8_-O0hmse7cbxiciHHCwOLA2ZzCNVMnkG0ryY2iMNAOIsAwuPl_ZvQ_0ZLmKSUj?key=2Yj3j6m_mrGSAHOLnVn3pg)

**Мобильная версия**

[Баг можно посмотреть тут](https://drive.google.com/file/d/1p8_P61W_iYUY4YpbphRv6vI8NuEYgvMs/view?usp=sharing)

### Ожидаемый результат

При изменении масштаба со 100% до 320% или изменения формата на мобильную версию, верстка не должна выходить за рамки контейнера или видимой области страницы.

### Окружение

Браузеры:

- Chrome. Версия 125.0.6422.61
- Яндекс. Версия 122.0.6261.952
- Mozilla Firefox. Версия 125.0.2 (64arm)

### Тестовое устройство

- Ноутбук ASUSTeK COMPUTER INC X550VB. Версия 1.0
- OS Linux Mint 20
- iPhone 12 mini (5,42 дюйма)

### Аналитика

Здесь оставляется ссылка на яндекс-метрику с количеством пользователей, которых задевает данная проблема.

### Серьёзность

- Minor
