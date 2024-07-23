# Не появляется фавикон на странице облачного диска и на странице авторизации

При загрузке страниц авторизации и облачного диска, появляется фоновая 404 ошибка, указывающая на отсутствие ресурса.

### Шаги воспроизведения

1. Перейти [по ссылке](http://cloud.hh-demo.np-internal.ru/) в одном из браузере (Firefox, Яндекс, Chrome);
2. Открыть DevTools, перейти во вкладку Network;
3. Перезагрузить страницу, найти ошибку 404 “Not Found”;
4. Заполнить логин и пароль (логин: napopravku, пароль: adminNaPopravku);
5. Нажать кнопку “Log in”;
6. Перезагрузить страницу;
7. Открыть DevTools, перейти во вкладку Network;
8. Найти ошибку 404 “Not Found”.

### Текущий результат

Фавикон не отображается - появляется ошибка.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcSO-PZzoQ-JBjpMWNW1C93FlKPzczASo3dwq89wPSUKTxcuPjMlQZ0RU9j5fTG9y7K-IjmpwI64AYBrS5VSpReTTvvVk3yfLFdD7fJTsZlR4uTFprBkm97HtGW2ddIr_Um_4S_zb6zDbeqk_7oqCVmbR8?key=UEFrhbNa-SPP1mkQX-45AA)

### Ожидаемый результат

Фавикон отображается корректно и там, где предусматривает согласованный дизайн. Фоновых ошибок при загрузке страницы нет.

### Окружение

Браузеры:

- Google Chrome. Версия 125.0.6422.61
- Яндекс. Версия 122.0.6261.952
- Mozilla Firefox. Версия 125.0.2 (64arm)

### Тестовое устройство

- Ноутбук ASUSTeK COMPUTER INC X550VB. Версия 1.0
- OS Linux Mint 20

### cURL запроса

```bash
curl "http://cloud.hh-demo.np-internal.ru/favicon.ico" --compressed -H "User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:128.0) Gecko/20100101 Firefox/128.0" -H "Accept: image/avif,image/webp,image/png,image/svg+xml,image/*;q=0.8,*/*;q=0.5" -H "Accept-Language: ru-RU,ru;q=0.8,en-US;q=0.5,en;q=0.3" -H "Accept-Encoding: gzip, deflate" -H "DNT: 1" -H "Connection: keep-alive" -H "Referer: http://cloud.hh-demo.np-internal.ru/" -H "Priority: u=6" -H "Pragma: no-cache" -H "Cache-Control: no-cache"
```

### Аналитика

Если бы я у Вас работала, то прикрепила бы ссылку на яндекс-метрику (или другую Вашу метрику) с количеством пользователей, которых задевает данная проблема.

### Документация

Если бы я у Вас работала, то прикрепила бы ссылку на документацию.

### Логи

Если бы я у Вас работала, то прикрепила бы ссылку на Kibana и Sentry.

### Slack

Если бы я у Вас работала и эту проблему уже обсуждали ранее, я бы прикрепила переписку обсуждения этого бага.

### Серьёзность

- Minor
