# MariaDBExample
A docker image which will deploy a mariadb container and runs some scripts to create and populate some tables for sql teaching purposes.

We can run a blank MariaDB system using
> docker run --name mariadbtest MYSQL\_ROOT\_PASSWORD=password -d mariadb/server:10.3

This will launch MariaDB in the background, and we can access it using
> docker exec -it mariadbtest bash

A bash shell is launched with root privileges, we can *cd*, *ls*, and even install file editors such as vim.  Once the bash shell is launched, we get into MariaDB in the usual way:
> mysql -u root -p
