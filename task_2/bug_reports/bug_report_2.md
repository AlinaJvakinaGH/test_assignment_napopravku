# Не работает кнопка  “Log Out”, на странице авторизации и облачного диска

При нажатии на кнопку “Log Out”, страница авторизации и облачного диска перезагружается и появляется страница “Хмм. Нам не удаётся найти этот сайт.” с 302 ошибкой.

### Шаги воспроизведения на странице авторизации

1. Перейти [по ссылке](http://cloud.hh-demo.np-internal.ru/) в одном из браузере (Firefox, Яндекс, Chrome);
2. Нажать кнопку “Log Out”.

### Шаги воспроизведения на странице облачного диска

1. Перейти [по ссылке](http://cloud.hh-demo.np-internal.ru/) в одном из браузере (Firefox, Яндекс, Chrome);
2. Заполнить логин и пароль (логин: napopravku, пароль: adminNaPopravku);
3. Нажать кнопку “Log in”;
4. Проскролить до футера страницы;
5. Нажать кнопку “Log Out”.

### Текущий результат на странице авторизации

[Баг можно посмотреть тут](https://drive.google.com/file/d/1jPnaWaLumD9GPNmvJ4dTCBeausV_oX0p/view?usp=sharing)

### Текущий результат на странице облачного диска

[Баг можно посмотреть тут](https://drive.google.com/file/d/1sslLpr7kEma4cnDH2aw3JCEOaVJDHneb/view?usp=sharing)

### Ожидаемый результат

При нажатии на кнопку “Log Out” пользователь должен быть корректно разлогинен и перенаправлен на страницу авторизации без отображения ошибки.

### Окружение

Браузеры:

- Google Chrome. Версия 125.0.6422.61
- Яндекс. Версия 122.0.6261.952
- Mozilla Firefox. Версия 125.0.2 (64arm)

### Тестовое устройство

- Ноутбук ASUSTeK COMPUTER INC X550VB. Версия 1.0
- OS Linux Mint 20
- iPhone 12 mini (5,42 дюйма)

### cURL запроса на странице авторизации

```bash
curl "http://cloud.hh-demo.np-internal.ru/php/auth.php?logout=true" -H "User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:128.0) Gecko/20100101 Firefox/128.0" -H "Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/png,image/svg+xml,*/*;q=0.8" -H "Accept-Language: ru-RU,ru;q=0.8,en-US;q=0.5,en;q=0.3" -H "Accept-Encoding: gzip, deflate" -H "DNT: 1" -H "Connection: keep-alive" -H "Referer: http://cloud.hh-demo.np-internal.ru/" -H "Upgrade-Insecure-Requests: 1" -H "Priority: u=0, i" -H "Pragma: no-cache" -H "Cache-Control: no-cache"
```

### cURL запроса на странице облачного диска

```bash
curl "http://cloud.hh-demo.np-internal.ru/php/auth.php?logout=true" -H "User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:128.0) Gecko/20100101 Firefox/128.0" -H "Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/png,image/svg+xml,*/*;q=0.8" -H "Accept-Language: ru-RU,ru;q=0.8,en-US;q=0.5,en;q=0.3" -H "Accept-Encoding: gzip, deflate" -H "DNT: 1" -H "Connection: keep-alive" -H "Referer: http://cloud.hh-demo.np-internal.ru/" -H "Cookie: user__password=adminNaPopravku; user__name=napopravku; user__id=2; user__loggedin=1" -H "Upgrade-Insecure-Requests: 1" -H "Priority: u=0, i" -H "Pragma: no-cache" -H "Cache-Control: no-cache"
```

### Аналитика

Если бы я у Вас работала, то прикрепила бы ссылку на яндекс-метрику (или другую Вашу метрику) с количеством пользователей, которых задевает данная проблема.

### Документация

Если бы я у Вас работала, то прикрепила бы ссылку на документацию к фиче.

### Логи

Если бы я у Вас работала, то прикрепила бы ссылку на Kibana и Sentry.

### Slack

Если бы я у Вас работала и эту проблему уже обсуждали ранее, я бы прикрепила переписку обсуждения этого бага.

### Серьёзность

- Major
