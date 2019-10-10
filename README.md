# bltest

Распаковать, перейти в директорию, запустить :
```
docker-compose up
```

Проверка кластера, после запуска:
```
sudo docker exec cassandra0 nodetool status
```

Так же в директориях *cas0data* и *cas1data* должны появиться данные.

Подключение: 

cassandra0:
```
cqlsh --cqlversion=3.4.4 -u cassandra -p cassandra 127.0.0.1 9042
```

cassandra1:
```
cqlsh --cqlversion=3.4.4 -u cassandra -p cassandra 127.0.0.1 9142
```
