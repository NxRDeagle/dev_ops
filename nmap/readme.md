# Сканирование серверов при помощи nmap

Порядок выполнения работы:

Создаем новую папку (mkdir nmap)

Добавляем в нее файлы:

inventory.ini

pb_nmap.yml

targets.txt

Ред. файл .ini, содержащий ip ВМ, с которой происходит сканирование

В файле .yml записываем скрипт запускающий playbook

В файле .txt записываем адреса сканируемых серверов

Установка nmap (sudo apt install nmap)

Запуск playbook с выводом изменений и запросом пароля (ansible-playbook pb_nmap.yml -i inventory.ini --diff --ask-become-pass)
