# Домашнее задание "Система мониторинга Zabbix. Часть 2"

## Описание
В рамках домашнего задания был создан шаблон для мониторинга CPU и RAM, добавлены два хоста с Zabbix Agent, создан кастомный дашборд.

## Выполненные задания

### Задание 1
Создан шаблон `Template OS CPU RAM Custom` с элементами данных:
- **CPU utilization percentage** (key: `system.cpu.load[percpu,avg1]`)
- **RAM utilization percentage** (key: `vm.memory.size[pused]`)

![Задание 1](screenshots/zadanie-1.png)

### Задание 2-3
Добавлены два хоста:
- `ivanovii-1` (IP: 127.0.0.1)
- `ivanovii-2` (IP: 192.168.0.140)

Привязанные шаблоны:
- `Linux by Zabbix agent`
- `Template OS CPU RAM Custom`

Статус: **ZBX (зелёный)**

![Задание 2-3](screenshots/zadanie-2-3.png)

### Задание 4
Создан дашборд **"CPU and RAM Dashboard"** с графиками CPU и RAM.

![Задание 4](screenshots/zadanie-4.png)

