# codespace-lamp
Aggiorna repository e controlla versioni aggiornate
$sudo apt update
$sudo apt upgrade

Installazione lamp server
$sudo apt install lamp-server^

Avviare il servizio apache
$sudo service apache2 start

Avviare il servizio mysql
$sudo service mysql start

Installazione phpmyadmin
$sudo apt-get install phpmyadmin

Includere la seguente riga alla fine del file /etc/apache2/apache2.conf
    Include /etc/phpmyadmin/apache.conf  

Riavviare apache
$sudo service apache2 restart

Individuare le credenziali di default nel file /etc/mysql/debian.cnf (username e password di default per mysql)
Accedere a mysql con le credenziali di default
Mmodificare la password di root
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'TUA_PASSWORD';
Accedere con la password di root

Abilita la porta 80 e rendi il link pubblico
