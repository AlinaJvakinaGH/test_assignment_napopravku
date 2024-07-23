# Созданные папки не отображаются в UI облачного диска

После нажатия на кнопку “Add Folder” и присвоении папке имени страница перезагружается, но новая папка в UI облачного диска не создаётся.

### Шаги воспроизведения

1. Перейти [по ссылке](http://cloud.hh-demo.np-internal.ru/) в одном из браузере (Firefox, Яндекс, Chrome);
2. Заполнить логин и пароль (логин: napopravku, пароль: adminNaPopravku);
3. Нажать кнопку “Log In”;
4. Проскролить до футера страницы;
5. Нажать кнопку “Add Folder”;
6. Присвоить папке любое имя;
7. Подтвердить.

### Текущий результат

При создании папки происходит перезагрузка страницы. Отправляется POST запрос с названием папки и идентификатором родительской папки, после чего приходит ответ со статусом кодом “200” с текстом "Folder was successfully added". Но в IU папка не появляется.

[Посмотреть баг тут](https://drive.google.com/file/d/1eNNog8nzXLtrQnoL_H-eIAkjxea-wjow/view?usp=sharing)

### Ожидаемый результат

После нажатия на кнопку “Add Folder” и успешного создания новой папки, она должна отображаться в пользовательском интерфейсе облачного диска. Пользователь должен видеть новую папку с присвоенным именем.

### Окружение

Браузеры:

- Google Chrome. Версия 125.0.6422.61
- Яндекс. Версия 122.0.6261.952
- Mozilla Firefox. Версия 125.0.2 (64arm)

### Тестовое устройство

- Ноутбук ASUSTeK COMPUTER INC X550VB. Версия 1.0
- OS Linux Mint 20
- iPhone 12 mini (5,42 дюйма)

### cURL запроса

```bash
curl "http://cloud.hh-demo.np-internal.ru/php/upload.php" -X POST -H "User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:128.0) Gecko/20100101 Firefox/128.0" -H "Accept: */*" -H "Accept-Language: ru-RU,ru;q=0.8,en-US;q=0.5,en;q=0.3" -H "Accept-Encoding: gzip, deflate" -H "Content-Type: multipart/form-data; boundary=---------------------------6870745628193552962350940739" -H "Origin: http://cloud.hh-demo.np-internal.ru" -H "DNT: 1" -H "Connection: keep-alive" -H "Referer: http://cloud.hh-demo.np-internal.ru/" -H "Cookie: user__password=adminNaPopravku; user__name=napopravku; user__id=2; user__loggedin=1" -H "Priority: u=0" -H "Pragma: no-cache" -H "Cache-Control: no-cache" --data-binary $'-----------------------------6870745628193552962350940739\r\nContent-Disposition: form-data; name="add_folder"\r\n\r\ntrue\r\n-----------------------------6870745628193552962350940739\r\nContent-Disposition: form-data; name="add_folder__name"\r\n\r\nNew Folder \u2116 1\r\n-----------------------------6870745628193552962350940739\r\nContent-Disposition: form-data; name="parent_folder__id"\r\n\r\n1\r\n-----------------------------6870745628193552962350940739--\r\n'
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
