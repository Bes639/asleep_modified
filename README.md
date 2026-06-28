```
                      ASLEEP SCANNER (MODIFIED)
```
[![Python](https://img.shields.io/badge/Python-3.6%2B-blue?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Version](https://img.shields.io/badge/Version-0.1_Beta-purple?style=for-the-badge)](https://github.com/)
[![Telegram](https://img.shields.io/badge/Telegram-@SniffCam-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/SniffCam)

Установка и запуск
------------------------------------------------------------------------
1. Клонируйте репозиторий:
   ```bash
   git clone https://github.com/Bes639/asleep_modified.git
   cd asleep_modified
   ```
2. Установка зависимости:
   ```bash
   pip3 install -r requirements.txt
   ```
4. Запуск сканера:
   ```bash
   python3 asleep.py
   ```
Инструкция и использования asleep
------------------------------------------------------------------------
```bash
   $ asleep.py [-h] [-s SCAN_FILE] [-p PORTS] [-b BRUTE_FILE] [-l] [-m] [-t THREADS] [-d]
               [--masscan-resume] [--no-snapshots] [--no-xml] [--dead] [--country] [--random-country]

АРГУМЕНТЫ
   -h, --help        показать это справочное сообщение и выйти
   -s SCAN_FILE      файл с диапазонами IP-адресов для сканирования, например: 192.168.1.1-192.168.11.1
   -p PORTS          порты для сканирования (по умолчанию: 37777), например: 37777,37778
   -b BRUTE_FILE     файл с IP-адресами для брутфорса, в любом формате
   -l                брутить комбинации из logins.txt и passwords.txt вместо combinations.txt
   -m, --masscan     запустить Masscan и сбрутить результаты
   -t THREADS        количество потоков для Masscan (по умолчанию: 3000)
   --masscan-resume  продолжить приостановленное сканирование Masscan
   --no-snapshots    не делать снимки (скриншоты)
   --no-xml          не создавать файлы .xml для SMART PSS
   --dead            записывать несбрученные камеры в файл dead_cams.txt
   --country         сканировать по конкретной стране
   --random-country  сканировать по случайной стране
   -d, --debug       вывод отладочной информации

ПРИМЕРЫ
   $ ./asleep -m -s ips.txt
   $ ./asleep -m -s ips.txt -p 37777,37778,47777
   $ ./asleep --country
   $ ./asleep --random-country
   $ ./asleep -b ips.txt
```
------------------------------------------------------------------------
Этот инструмент разработан исключительно в проверки безопасности своих камер и для 
проведения авторизованного аудита безопасности. Автор не несет 
ответственности за любой ущерб, причиненный использованием данного 
ПО в неправомерных целях.
========================================================================

Автор модификации
-----------------
Bes639
Telegram канал: @SniffCam

Поставьте звезду проекту на GitHub если вам понравился мой проект, мне будет приятное
