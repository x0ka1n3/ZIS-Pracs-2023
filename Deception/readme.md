# Deception
## Запуск контейнера
![](assets/1.png)

## Запуск хакерской активности
![](assets/2.png)

## Запуск сканирования nmap'ом
### sudo nmap localhost -A -sS -O -p0- -vvv
![](assets/3.png)

## Найденные запущенные службы
### FTP
![](assets/4.1.png)
### Команды, найденные в логах
![](assets/9.png)

	Происходит логин с anonymous:anonymous
	Вывод на экран текущей директории
	Загрузка на сервер скрипта exploit.sh
	Замена файла /etc/passwd

### SSH
![](assets/4.2.png)
### Команды, найденные в логах
![](assets/6.png)

	cd / - Переход в корневую директорию
	ss -tunlp - Вывод открытых портов и запущенных служб
	ls -la - Просмотр текущей директории
	whoami - Вывод имени текущего пользователя

### Telnet
![](assets/4.3.png)
### Команды, найденные в логах
![](assets/5.png)

	display arp - Вывод ARP таблицы
	display arp interface GigabitEthernet 0/0/1 - Вывод информации интерфейса gi0/0/1

### HTTP
![](assets/4.4.png)
### Команды, найденные в логах
![](assets/6.png)

	Попытки через payload вызвать различные методы сервера

### Redis
![](assets/4.5.png)
### Команды, найденные в логах
![](assets/7.png)

	Попытка вывести информацию о клиентах, админе и ключах