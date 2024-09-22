Лабораторная работа №15 по курсу Linux Pro.

Задание:
	Настроить дашборд с 4-мя графиками:
		память;
		процессор;
		диск;
		сеть.


Решение:

1) Развернута виртуальная машина с помощью Vagrant ОС Ubuntu 22.04
2) Установлен Zabbix, собран дашборд из метрик собранных с Zabbix сервера (см Zabbix.jpg)
3) Установлен Prometheus
4) Node Exporter развернут на материнской ОС, в конфиг Prometheus добавлено задание (см Prometheus.jpg)
5) Установлена Grafana, на основе метрик Prometheus собран дашборд (см Grafana.jpg)
6) Grafama & Prometheus systemctl.jpg показывает состояние служб Grafana и Prometheus
7) В Docker'е  развернут Graphite и подключен к Grafana (см Graphite Datasource.jpg)
8) На основе метрик Graphite собран дашборд (см Graphite Dashboard.jpg)