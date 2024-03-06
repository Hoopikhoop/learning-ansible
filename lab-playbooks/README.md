# Ansible Playbooks

1. Добавь в playbook еще один task. Этот новый task должен выполнять команду cat /etc/hosts и его название должно быть Execute a command to display hosts file
2. Мы запустили и проверили все эти tasks на localhost. Теперь мы хотим запустить их в боевой среде на хосте web_node1. Обнови этот play, чтобы запуск был на узле web_node1.
3. Изучи прикрепленный inventory-файл. Нам требуется запустить tasks определенные в play на серверах, которые территориально находятся в boston. Отрази эти сервера в playbook.
4. Создай новый play с названием Execute a command to display hosts file contents on web_node2, который выполнит команду cat /etc/hosts на ноде web_node2, a название task должно быть Execute a command to display hosts file.
5. Останови web-службы на веб-серверах
Останови db-службы на серверах баз данных
Перегрузи все сервера (web и db) за один раз
Запусти db-службы на узлах баз данных
Запусти web-службы на узлах веб-серверов