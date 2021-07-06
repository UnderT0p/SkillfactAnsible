# SkillfactAnsible
14.4 

Написать свой Playbook, который будет устанавливать и запускать Docker на локальной машине.

Написать свой Playbook, который будет запускать MySQL-сервер на локальной машине

14.5.1 

14.5.1.yaml - добавляет пользователя на машину указанную в hosts.txt и копирует из папки файл id_rsa.pub(закодированный в vault)

команда:
 ansible-playbook 14.5.1.yaml -i hosts.txt --ask-vault-pass
 
 postfix.yaml - устанавливает, либо удаляет почтовый сервер postfix в зависимости от тега(в задании специально приведена не верная команда, имею ввиду порядокключей?)
 
 ansible-playbook -t 'init postfix' postfix.yaml -i hosts.txt
 
 ansible-playbook -t 'drop postfix' postfix.yaml -i hosts.txt


14.6.1

vsftpd - папка с ролью, в ней привел то, куда вносил изменения

ftp.yaml - playbook с роью

hosts - адрес хоста

status_ftp.png - скрин запущенного сервиса фтп на целевой машине.
