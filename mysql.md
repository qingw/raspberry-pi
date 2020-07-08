# sudo apt-get install mysql-server 

# vi /etc/mysql/mysql.conf.d/mysqld.cnf
bind-address            = 0.0.0.0

use mysql;


# 使用mysql 数据库
mysql > use mysql;
-- 修改密码
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'root';
ALTER USER 'root'@'%' IDENTIFIED WITH mysql_native_password BY 'root';

# 特定用户的host 修改
mysql > update user set host='%' where user='root';
# 指定用户的授权
mysql > grant all privileges on *.* to root@'%'


FLUSH PRIVILEGES;

在[mysqld]中添加下边的代码
default_authentication_plugin=mysql_native_password

然后重启MySQL
service mysqld restart


/opt/zookeeper   
192.168.1.8  
