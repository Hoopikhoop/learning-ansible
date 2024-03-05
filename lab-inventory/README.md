# Ansible Inventory

1. Наши вебсерверы на Linux, но сервер базы данных на Windows. Добавь дополнительные параметры в каждую строку, чтобы были ansible_connection, ansible_user и password.
2. Мы создали группу вебсерверов. Таким же образом создай группу для серверов баз данных с названием db_servers и добавь туда сервер db1.
3. Создай группу с названием all_servers и добавь в нее ранее созданные группы web_servers и db_servers.
4. Попробуй представить приведенные ниже в таблице данные в формате Ansible Inventory

Server Alias	Server Name	OS	User	Password
sql_db1	sql01.xyz.com	Linux	root	Lin$Pass
sql_db2	sql02.xyz.com	Linux	root	Lin$Pass
web_node1	web01.xyz.com	Win	administrator	Win$Pass
web_node2	web02.xyz.com	Win	administrator	Win$Pass
web_node3	web03.xyz.com	Win	administrator	Win$Pass

Сгруппируй серверы на основе этой таблицы:

Group	Members
db_nodes	sql_db1, sql_db2
web_nodes	web_node1, web_node2, web_node3
boston_nodes	sql_db1, web_node1
dallas_nodes	sql_db2, web_node2, web_node3
us_nodes	boston_nodes, dallas_nodes