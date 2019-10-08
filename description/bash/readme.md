# Элиас bash [(back)](./readme.md)

## Файлы

- **sl** => `ls`
- **ll** => `ls -lah` # Показать скрытые файлы с читаемыми размерами
- **l.** => `ls -d .*` # Показать только скрытые файлы и папки
- **lf** => `ls -p | grep -v /` # Показать только файлы
- **ld** => `ls -d */` # Показать только директории
- **lt** => `ls -lhart` # Сортировать по времени
- **lz** => `ls -AFlSr` # Сортировать по размеру
- **t** => `touch`
- **ff** => `find . -type f -iname` # Найти файл по имени в текущей папке
- **catc** => `clear && grep -v -e "^$" -e"^ *#"` # Показать файл с кодом без коментариев

## Директории

- **md** => `mkdir -pv`
- **fd** => `find . -type d -name` # Найти директорию по имени в текущей папке
- **..** => `cd ..`
- **...** => `cd ../..`
- **.3** => `cd ../../..`
- **.4** => `cd ../../../..`
- **g** => `cd /`
- **w** => `cd /var/www`
- **bscript** => `cd /usr/local/sbin && ls` # Показать список своих Bash-скриптов
- **ngsa** => `cd /etc/nginx/sites-enabled && ls` # Показать список доступных сайтов в nginx

## Архивы

- **tarc** => `tar czvf` # Создать архив
- **tarx** => `tar xzvf` # Извлечь архив
- **tart** => `tar tzvf` # Показать содержимое архива

## Подтверждение действий

- **mv** => `mv -iv`
- **cp** => `cp -iv`
- **ln** => `sudo ln -iv`
- **rm** => `sudo rm -riv`
- **rmf** => `sudo rm -rfiv` # Принудительное удаление

## Обновление Bash-файлов

- **bau** => `. ~/.bash_aliases`
- **bpu** => `. ~/.bash_profile`
- **bru** => `. ~/.bashrc`

## Менеджер пакетов Apt (Ubuntu)

- **ag** => `sudo apt-get`
- **agi** => `sudo apt-get install`
- **agyi** => `sudo apt-get -y install`
- **agu** => `sudo apt-get update`
- **agr** => `sudo apt-get remove`
- **acs** => `apt-cache search`

## System info

- **df** => `df -hPT | column -t` # Память диска
- **free** => `free -mth` # RAM
- **path** => `echo $PATH | tr ':' '\n' | nl` # Удобный вывод $PATH

## Network

- **ping** => `ping -c4`
- **ports** => `netstat -tulanp` # Показать открытые порты
- **ipinfo** => `curl ifconfig.me && curl ifconfig.me/host` # Показать свой IP и Hostname

## Сокращения

- **q** => `exit`
- **s** => `sudo`
- **c** => `clear`
- **a** => `clear && - **| less` # Показать список алиасов
- **ag** => `- **| grep` # Если помнишь только часть имени алиаса

## Extra

- **ax** => `chmod a+x` # Сделать файлы исполняемым
