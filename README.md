# HW-10.3-Grafana

## Задание 1

Решение задания - скриншот веб-интерфейса grafana со списком подключенных Datasource.

![data source](https://github.com/olegrovenskiy/HW-10.3-Grafana/blob/main/%D0%BF%D1%83%D0%BD%D0%BA%D1%82%201.png)

## Задание 2

1. Утилизация CPU для nodeexporter (в процентах, 100-idle)
100-(node_load1{instance="nodeexporter:9100",job="nodeexporter"})/4*100

2. CPULA 1/5/15
node_load1{instance="nodeexporter:9100",job="nodeexporter"}
node_load5{instance="nodeexporter:9100",job="nodeexporter"}
node_load15{instance="nodeexporter:9100",job="nodeexporter"}

3. Количество свободной оперативной памяти
node_memory_MemFree_bytes{instance="nodeexporter:9100",job="nodeexporter"}

4. Количество места на файловой системе
node_filesystem_avail_bytes{device="/dev/sdb", fstype="ext4", instance="nodeexporter:9100", job="nodeexporter", mountpoint="/mnt"}

![dashboard](https://github.com/olegrovenskiy/HW-10.3-Grafana/blob/main/%D0%BF%D1%83%D0%BD%D0%BA%D1%82%202.png)

## Задание 3

Создайте для каждой Dashboard подходящее правило alert (можно обратиться к первой лекции в блоке "Мониторинг").

Для решения ДЗ - приведите скриншот вашей итоговой Dashboard.

![alerts](https://github.com/olegrovenskiy/HW-10.3-Grafana/blob/main/%D0%BF%D1%83%D0%BD%D0%BA%D1%82%203.png)


