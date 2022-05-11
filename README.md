# DevTips
How to mysql password?
1. Find mysql config file 'my.cnf' 
2. Add 'skip-grant-tables' uder [mysqld]
3. Restart Mysql
4. open terminal amd run 'mysql -u root -p' and this will allow to get into mysql without any password
5. From mysql terminal run 'flush privileges;
6. ALTER USER 'root'@'localhost' IDENTIFIED BY 'newpassword';
7. Exit from mysql terminal
8. open the my.cnf file again and delete 'skip-grant-tables'
9. save and exit the file
10. Now login again to mysql with new password 'mysql -uroot -pnewpassword';

Thats it!!!!!!!!!!!!!!!!!