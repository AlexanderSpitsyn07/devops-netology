# Домашнее задание к занятию "10.03. Grafana"

## Обязательные задания

### Задание 1
Используя директорию [help](./help) внутри данного домашнего задания - запустите связку prometheus-grafana.

![Screenshot](1-1.png)

Зайдите в веб-интерфейс графана, используя авторизационные данные, указанные в манифесте docker-compose.

![Screenshot](1-2.png)

Подключите поднятый вами prometheus как источник данных.

![Screenshot](1-3.png)

Решение домашнего задания - скриншот веб-интерфейса grafana со списком подключенных Datasource.

![Screenshot](1-4.png)


## Задание 2
Изучите самостоятельно ресурсы:
- [promql-for-humans](https://timber.io/blog/promql-for-humans/#cpu-usage-by-instance)
- [understanding prometheus cpu metrics](https://www.robustperception.io/understanding-machine-cpu-usage)

Создайте Dashboard и в ней создайте следующие Panels:
- Утилизация CPU для nodeexporter (в процентах, 100-idle)
- CPULA 1/5/15
- Количество свободной оперативной памяти
- Количество места на файловой системе

node_memory_MemFree_bytes

node_load1
node_load5
node_load15

node_cpu_seconds_total

node_filesystem_avail_bytes

Для решения данного ДЗ приведите promql запросы для выдачи этих метрик, а также скриншот получившейся Dashboard.

![Screenshot](2-2.png)

## Задание 3
Создайте для каждой Dashboard подходящее правило alert (можно обратиться к первой лекции в блоке "Мониторинг").

Для решения ДЗ - приведите скриншот вашей итоговой Dashboard.

![Screenshot](3-1-1.png)
![Screenshot](3-1-2.png)
![Screenshot](3-1-3.png)
![Screenshot](3-2.png)


## Задание 4
Сохраните ваш Dashboard.

Для этого перейдите в настройки Dashboard, выберите в боковом меню "JSON MODEL".

Далее скопируйте отображаемое json-содержимое в отдельный файл и сохраните его.

В решении задания - приведите листинг этого файла.

MyDash - Grafana




