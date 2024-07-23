# После нажатия на кнопку “Remove” в облачном диске появляется ошибка 304

При нажати на кнопку “Remove”, происходит перезагрузка страницы. После появляется страница “Хмм. Нам не удаётся найти этот сайт.” со статус кодом 304.

### Шаги воспроизведения

1. Перейти [по ссылке](http://cloud.hh-demo.np-internal.ru/) в одном из браузере (Firefox, Яндекс, Chrome);
2. Заполнить логин и пароль (логин: napopravku, пароль: adminNaPopravku);
3. Нажать кнопку “Log in”;
4. Нажать кнопку “Remove” у любого файла.

### Текущий результат

[Посмотреть баг тут](https://drive.google.com/file/d/1UQSAushcfVukjDdwBnL_ERM9BBKNHhRQ/view?usp=sharing)

### Ожидаемый результат

При нажатии на кнопку “Remove” файл должен корректно удаляться, оставаясь на главной странице облачного диска без отображения ошибок.

### Окружение

Браузеры:

- Google Chrome. Версия 125.0.6422.61
- Яндекс. Версия 122.0.6261.952
- Mozilla Firefox. Версия 125.0.2 (64arm)

### Тестовое устройство

- Ноутбук ASUSTeK COMPUTER INC X550VB. Версия 1.0
- OS Linux Mint 20
- iPhone 12 mini (5,42 дюйма)

### curl запроса

curl '<http://cloud.hh-demo.np-internal.ru/php/remove.php?remove_file__id=8501>' -H 'User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:128.0) Gecko/20100101 Firefox/128.0' -H 'Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/png,image/svg+xml,*/*;q=0.8' -H 'Accept-Language: ru-RU,ru;q=0.8,en-US;q=0.5,en;q=0.3' -H 'Accept-Encoding: gzip, deflate' -H 'DNT: 1' -H 'Connection: keep-alive' -H 'Referer: <http://cloud.hh-demo.np-internal.ru/>' -H 'Cookie: user__password=adminNaPopravku; user__name=napopravku; user__id=2; user__loggedin=1' -H 'Upgrade-Insecure-Requests: 1' -H 'Priority: u=0, i' -H 'Pragma: no-cache' -H 'Cache-Control: no-cache'

### Аналитика

Если бы я у Вас работала, то прикрепила бы ссылку на яндекс-метрику (или другую Вашу метрику) с количеством пользователей, которых задевает данная проблема.

### Документация

Если бы я у Вас работала, то прикрепила бы ссылку на документацию к фиче.

### Логи

Если бы я у Вас работала, то прикрепила бы ссылку на Kibana и Sentry.

### Slack

Если бы я у Вас работала и эту проблему уже обсуждали ранее, я бы прикрепила переписку обсуждения этого бага.

### Серьёзность

- Critical
