### 1. Опишите основные плюсы и минусы pull и push систем мониторинга.

PUSH:

1. упрощённая репликация(резервирование) данных
2. гибкая настройка отправки. (разные данные на разные хосты)
3. используется UDP, который легче для сети.

PULL:

1. легче контроллировать подлинность данных. можно с разных серверов опрашивать разные агенты.
2. возможность настроить tls для безопасного обмена данными
3. упрощённая отладка получения данных с агентов (можно сторонним софтом опрашивать агенты через http)

### 2. Какие из ниже перечисленных систем относятся к push модели, а какие к pull? А может есть гибридные?

* Prometheus - PULL/PUSH
* TICK - PUSH
* Zabbix - PULL/PUSH
* VictoriaMetrics - TSDB
* Nagios - PULL

### 3.

* [curl http://localhost:8086/ping](curl-8086.png)
* [curl http://localhost:8888](curl-8888.png)
* [curl http://localhost:9092/kapacitor/v1/ping](curl-9092.png)

### 4.
[disk metrics screen](disk-util.png)

### 5.
[docker metrics screen](docker-metrics.png)
