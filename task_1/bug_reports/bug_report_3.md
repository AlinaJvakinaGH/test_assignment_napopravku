
# На странице заполнения профиля заголовок “Заполните свой профиль и получите 100 баллов” при изменении масштаба выходит за границы блока

При изменении масштаба с 100% до минимального разрешения экрана (320%) заголовок “Заполните свой профиль и получите 100 баллов” в основном блоке выходит за его рамки.

### Шаги воспроизведения на десктопной версии

1. Перейти по [ссылке](http://landing.hh-demo.np-internal.ru/) в одном из трёх браузеров (Chrome, Яндекс, Mozilla Firefox);
2. Изменить масштаб страницы со 100% до 320%.

### Шаги воспроизведения на мобильной версии

1. На телефонне перейти по [ссылке](http://landing.hh-demo.np-internal.ru/) в одном из трёх браузеров (Chrome, Яндекс, Mozilla Firefox);
2. Сравнить вёрстку с макетом в фигме.

### Текущий результат

**десктоп версия:**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXf5F-Pc0K7HdpOQThcLqDwLxQE5u9oSdPTscTKRm9GbsIj_sKYtLoY6ZBCs7Zx8GF_v4oc4g6Y7fynZX8LKeKTBf-OcORSBMzPw-X8ta2GIeVIF0zfZlijezQTPVTaBnVUnUnnQRyWR13UD5kW4aVuHCsy4?key=XObOV-jfI8ziYNcxe3MVfg)

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXe_2JrFYs22nOhAGWpBWOpZ7Ap3DsmeFWvMn36ooCzW5Y5RwJb3JVOzufp0icKMg97aVLQ3Za9WWyCjo5xeS_I1yGBF9JfeI2XIqmvh_au24pa57qNxcdReJ0fWIJbKhbaZ0M_-Y4Lpm8TFHsGd5ifKL5OF?key=XObOV-jfI8ziYNcxe3MVfg)

**Мобильная версия**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXf2_LLKRZkToEwIjtFJuCiwaNSgV338ezcg5ou1ttFpqO_7oKDO08gUixQyoemW7v3q1EtcZ0obEzirI7swp2hTeftK6XFC5CoN0-jq4CEietNC3-oZv0ZNohSpkKAoL8JOssOhOb_i0P0bdJa6DTgUXhWA?key=XObOV-jfI8ziYNcxe3MVfg)

### Ожидаемый результат

При изменении масштаба со 100% до 320% или изменения формата на мобильную версию, верстка не должна выходить за рамки блока или видимой области страницы.

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

Здесь должна быть ссылка на яндекс-метрику (или другую Вашу метрику) с количеством пользователей, которых задевает данная проблема.

### Серьёзность

- Minor
