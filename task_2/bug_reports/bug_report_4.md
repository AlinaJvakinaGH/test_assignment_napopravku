# Нельзя загрузить в облачный диск файл, вес которого превышает 1048KB

При загрузке файлов с весом больше 1049KB в облачный диск, происходит 413 ошибка “Request Entity Too Large”.

### Шаги воспроизведения

1. Перейти [по ссылке](http://cloud.hh-demo.np-internal.ru/) в одном из браузере (Firefox, Яндекс, Chrome);
2. Заполнить логин и пароль (логин: napopravku, пароль: adminNaPopravku);
3. Нажать кнопку “Log in”
4. Нажать кнопку “Обзор”;
5. Выбрать любой файл больше 1048KB (1,048MB);
6. Нажать кнопку “Upload File”.

### Текущий результат

При загрузке файлов происходит ошибка. Можно загрузить файлы любого формата, но только если вес одного (или всех в совокупности) файла не будет превышать 1049KB.

При загрузке файлов с весом больше 1049KB в облачный диск, происходит 413 ошибка “Request Entity Too Large”.

[Посмотреть баг тут](https://drive.google.com/file/d/1LXrGdfDXhpuveg0yA9mBWpHuMhYVO4Uz/view?usp=sharing)

### Ожидаемый результат

Облачный диск должен позволять загружать файлы весом до 7MB (или нескольких файлов с совокупным весом до 7MB) без возникновения ошибок.

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
curl "http://cloud.hh-demo.np-internal.ru/php/upload.php" -X POST -H "User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:128.0) Gecko/20100101 Firefox/128.0" -H "Accept: */*" -H "Accept-Language: ru-RU,ru;q=0.8,en-US;q=0.5,en;q=0.3" -H "Accept-Encoding: gzip, deflate" -H "Content-Type: multipart/form-data; boundary=---------------------------190da2b9f59" -H "Origin: http://cloud.hh-demo.np-internal.ru" -H "DNT: 1" -H "Connection: keep-alive" -H "Referer: http://cloud.hh-demo.np-internal.ru/" -H "Cookie: user__password=adminNaPopravku; user__name=napopravku; user__id=2; user__loggedin=1" -H "Pragma: no-cache" -H "Cache-Control: no-cache" --data-binary $'-----------------------------190da2b9f59\r\nContent-Disposition: form-data; name="files[]"; filename="ssssss.jpg"\r\nContent-Type: image/jpeg\r\n\r\n-----------------------------190da2b9f59--\r\n'
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

- Critical
