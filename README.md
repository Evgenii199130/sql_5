# sql_5

Задание 1
На лекции рассматривались режимы репликации master-slave, master-master, опишите их различия.

Ответ:

### Master-Slave Репликация

- Репликация: Односторонняя (от Master к Slaves).
- Запись: Только на Master.
- Чтение: На Master и Slaves.
- Отказоустойчивость: При сбое Master записи невозможны.
- Балансировка нагрузки: Чтение распределяется между Slaves.

### Master-Master Репликация

- Репликация: Двусторонняя (между всеми Masters).
- Запись: На любом из Masters.
- Чтение: На любом из Masters.
- Отказоустойчивость: При сбое одного Master другой продолжает работу.
- Конфликты: Возможны конфликты данных.
- Балансировка нагрузки: Чтение и запись распределяются между всеми Masters.

### Сравнение:

- Репликация: Master-Slave — односторонняя, Master-Master — двусторонняя.
- Запись: Master-Slave — только на Master, Master-Master — на любом Master.
- Чтение: Master-Slave — на Master и Slaves, Master-Master — на любом Master.
- Отказоустойчивость: Master-Slave — при сбое Master записи невозможны, Master-Master — при сбое одного Master другой продолжает работу.
- Конфликты: Master-Slave — нет, Master-Master — есть.
- Балансировка нагрузки: Master-Slave — чтение распределяется между Slaves, Master-Master — чтение и запись распределяются между всеми Masters.

Задание 2
Выполните конфигурацию master-slave репликации, примером можно пользоваться из лекции.

Приложите скриншоты конфигурации, выполнения работы: состояния и режимы работы серверов.

Ответ:

![1](https://github.com/Evgenii199130/sql_5/blob/main/scrin/sql_5.1.png)
![1](https://github.com/Evgenii199130/sql_5/blob/main/scrin/sql_5.2.png)
![1](https://github.com/Evgenii199130/sql_5/blob/main/scrin/sql_5.3.png)
![1](https://github.com/Evgenii199130/sql_5/blob/main/scrin/sql_5.4.png)
