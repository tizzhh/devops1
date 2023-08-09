# Part 1: <br>
![Part1](Part1.jpg) <br>

# Part 2: <br>
![Part2](Part2.jpg) <br>
![Part2.1](Part2.1.jpg) <br>
![Part2.2](Part2.2.jpg) <br>

# Part 3:
![Part3](Part3.jpg) <br>
sudo dpkg-reconfigure tzdata <br>
![Part3.1](Part3.1.jpg) <br>
In the report give an explanation for the presence of the lo interface: 
![Part3.2](Part3.2.jpg) <br>
lo - виртуальный интерфейс, используется для отладки сетевых программ и запуска серверных приложений на локальной машине. С этим интерфейсом всегда связан адрес 127.0.0.1. У него есть dns-имя – localhost. Любой трафик, который посылается компьютерной программой на интерфейс loopback, тут же получается тем же интерфейсом. Он всегда доступен, независимо от состояния физических сетевых интерфейсов. <br>
![Part3.3](Part3.3.jpg) <br>
DHCP назначает свободные IP-адреса для девайсов, отправляющих запрос на использование сети.
inet 10.0.2.15/24 brd 10.0.2.255 scope global dynamic enp0s3 - DHCP выделил адрес 10.0.2.15 для enp0s3. <br>
valid_lft 85101sec preferred_lft 85101sec - адрес валиден 85101 секунд.
![Part3.4](Part3.4.jpg) <br>
Internal: 10.0.2.2 <br>
External: 10.0.2.15 <br>
![Part3.5](Part3.5.jpg) <br>
![Part3.6](Part3.6.jpg) <br>
![Part3.7](Part3.7.jpg) <br>
# Part 4:
![Part4](Part4.jpg) <br>
# Part 5:
sudo нужно для выполнения команд от суперпользователя root (повышение привилегий), либо других пользователей.
![Part5](Part5.jpg) <br>
# Part 6:
![Part6](Part6.jpg) <br>
# Part 7:
Vim: 
1) vim test_vim.txt
2) i
3) hewettja
4) esc
5) wq + enter <br>
![Part7](Part7.jpg) <br>

Nano:
1) nano test_nano.txt
2) hewettja
3) Ctrl+O
4) Enter
5) Ctrl+X <br>
![Part7.1](Part7.1.jpg) <br>

MCEDIT:
1) mcedit test_mcedit.txt
2) hewettja
3) f2 + enter
4) f10 <br>
![Part7.2](Part7.2.jpg) <br>
![Part7.3](Part7.3.jpg) <br>

Vim:
1) shift + S
2) 21 School 21
3) esc
4) q! + enter <br>
![Part7.4](Part7.4.jpg) <br>

Nano:
1) ctrl + \
2) hewettja
3) 21 School 21
4) y + enter
5) Ctrl+X
6) N+enter <br>
![Part7.5](Part7.5.jpg) <br>

MCEDIT:
1) f4
2) hewettja + tab + 21 School 21
3) enter
4) f10
5) no <br>

Search:

![Part7.6](Part7.6.jpg) <br>
![Part7.7](Part7.7.jpg) <br>
![Part7.8](Part7.8.jpg) <br>
![Part7.9](Part7.9.jpg) <br>
![Part7.10](Part7.10.jpg) <br>
![Part7.11](Part7.11.jpg) <br>
![Part7.12](Part7.12.jpg) <br>
![Part7.13](Part7.13.jpg) <br>
![Part7.14](Part7.14.jpg) <br>
![Part7.15](Part7.15.jpg) <br>
![Part7.16](Part7.16.jpg) <br>
![Part7.17](Part7.17.jpg) <br>
![Part7.18](Part7.18.jpg) <br>
![Part7.19](Part7.19.jpg) <br>

# Part 8:

1)  - sudo apt update 
    - sudo apt install openssh-server
2) - sudo systemctl enable ssh
   - sudo systemctl start ssh
3) - sudo vim /etc/ssh/sshd_config
    - /Port enter
    - Port 2022
    - service sshd restart
4) - ps -ef | grep sshd
5) - sudo reboot

![Part8](Part8.jpg) <br>
ps : показывает процессы, -e выбирает все процессы, -f детальная информация
![Part8.1](Part8.1.jpg) <br>
-t: показывает tcp соединения, -a показывает активные и ожидающие соединения, включая слушающие порты, -n показывает адреса как числа

tcp: протокол соединения<br>
0 и 0: очереди получения и отправки данных на сокет<br>
0.0.0.0:2022: адрес и порт сервера<br>
0.0.0.0:*: адрес и порт клиента, * - любой порт<br>
LISTEN - состояние соединения, сервер "слушает" на указанном порту и ожидает входящих соединений

# Part 9:
![Part9](Part9.jpg) <br>
top:
- uptime: 56 mins
- number of authorised users: 1
- total system load: 0.03
- total number of processes: 104
- cpu load: 0.0 user, 0.2 system, 0.0 nice, 99.8 idle, 0.0 I/O wait, 0.0 hardware interrupts, 0.0 soft. interrupts, 0.0 stolen time
- memory load: 159.1 используется процессами, 402.4 используется для кэша
- pid of the process with the highest memory usage: 677
![Part9.1](Part9.1.jpg) <br>
- pid of the process taking the most CPU time: 1197

htop:
![Part9.2](Part9.2.jpg) <br>
![Part9.3](Part9.3.jpg) <br>
![Part9.4](Part9.4.jpg) <br>
![Part9.5](Part9.5.jpg) <br>
![Part9.6](Part9.6.jpg) <br>
![Part9.7](Part9.7.jpg) <br>
![Part9.8](Part9.8.jpg) <br>

# Part 10:

/dev/sda: 25 GiB, 52428800 sectors, 2GiB swap size

# Part 11:

![Part11](Part11.jpg) <br>
- partion size: 11758760
- space used: 4821296
- space free: 6318356
- percentage used: 44%
- measurement unit: 1024 бита

![Part11.1](Part11.1.jpg) <br>
- partion size: 12G
- space used: 4.6G
- space free: 6.1G
- percentage used: 44%
- file system type: ext4

# Part 12:

![Part12](Part12.jpg) <br>
![Part12.1](Part12.1.jpg) <br>

# Part 13:

![Part13](Part13.jpg) <br>
![Part13.1](Part13.1.jpg) <br>
![Part13.2](Part13.2.jpg) <br>
![Part13.3](Part13.3.jpg) <br>
![Part13.4](Part13.4.jpg) <br>
![Part13.5](Part13.5.jpg) <br>

# Part 14:

![Part14](Part14.jpg) <br>
17:53:29, hewettja, LOGIN
![Part14.1](Part14.1.jpg) <br>

# Part 15:

![Part15](Part15.jpg) <br>
![Part15.1](Part15.1.jpg) <br>
![Part15.2](Part15.2.jpg) <br>
![Part15.3](Part15.3.jpg) <br>
