## Сервис БД

#### Структура
```
database_service/
├──docker-compose.yml
└──.env
 ```

#### В директории "database_service" выполнить команды:

###### Собрать и запустить контейнер
```
docker-compose up -d --build
```

###### Остановить контейнер
```
docker-compose stop
```

###### Удалить контейнер
```
docker-compose down -v
```

- При подключении к БД из одной сети в [PG Admin](http://localhost:5050), на вкладке "Connection" указать значение <container_name> из docker-compose.yml (указывается имя контейнера postgres)
- При подключении к БД из другой сети указывается localhost (если контейнер развернут локально) или IP адрес удаленного сервера