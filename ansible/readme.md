# Ansible-playbook

Порядок выполнения работы:

В настройках ВМ в разделе "сеть" настраиваем виртуальный адаптер и NAT

Генерируем ключ в .ssh/authorized_keys

Скачиваем ansible (sudo apt install ansible)

Создаем директорию ansible_dir и вносим туда необходимые файлы:

mkdir ansible_dir
cd ansible_dir
index.html
playbook.yml

Редактриуем скрипты в index.html и playbook.yml

Запускаем скрипт (sudo ansible-playbook playbook.yml)

Вводим localhost в поисковик, после чего открывается разметка (прописана в index.html)
