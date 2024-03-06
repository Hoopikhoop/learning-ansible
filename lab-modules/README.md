# Ansible Modules

1. В playbook нужно добавить play для выполнения скрипта на всех веб-серверах. Название у play будет Execute a script on all web server nodes. Сам скрипт находится в размещении /tmp/install_script.sh
2. Измени playbook, добавив в него новый task, который запустит сервис httpd на всех web-хостах
3. Обнови playbook и добавь в него новый task, так, чтобы он был первым. Этот task должен вносить запись в файл /etc/resolv.conf для этих web_nodes. Строка, которую надо добавить: nameserver 10.1.250.10
4. Измени playbook и добавь в него новый task на вторую позицию (как раз после добавления строки в resolv.conf), который будет создавать нового пользователя на веб-сервере. Данные для добавления пользователя:
Username: web_user
uid: 1040
group: developers