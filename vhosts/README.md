# Создание виртуальных хостов с помощью ansible.

### Порядок выполнения работы:

- Создание каталога ansible_vhosts

* mkdir ansible_vhosts

- Наполнение каталога файлами

* inventory.ini (ip вм)
* playbook.yml (наименование роли и адреса сайтов для запуска скриптами)
* run_playbook.sh (скрипт shell, запускает playbook с запросом пароля)

- Создание каталога для ролей roles/nginx-vhosts
- Создание подкаталога handlers внутри roles/nginx-vhosts

* Внутри handlers создаем main.yml, который отвечает за рестарт nginx

- Создание подкаталога tasks внутри roles/nginx-vhosts

* Внутри tasks создаем main.yml, который отвечает за формирование сайтов в цикле

- Создание подкаталога templates внутри roles/nginx-vhosts

* Внутри templates прописываем код html (index.html.j2) и конфиг сервера (site.conf.j2)

- Запуск срипта shell

* sh run_playbook.sh
