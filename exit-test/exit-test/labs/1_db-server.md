yum install mariadb-server -y
service mariadb sto
service mariadb stop
vi /etc/my.cnf
systemctl enable mariadb
service mariadb start

yum install wget -y
wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-5.1.46.tar.gz
tar zxvf mysql-connector-java-5.1.46.tar.gz
mkdir /usr/share/java
cp mysql-connector-java-5.1.46/mysql-connector-java-5.1.46-bin.jar /usr/share/java/mysql-connector-java.jar

[root@ip-172-31-7-188 centos]# hostname -f
ip-172-31-7-188.ap-southeast-1.compute.internal


[root@ip-172-31-7-188 centos]# mysql -h ip-172-31-7-188.ap-southeast-1.compute.internal -u hive -p hive -e "status;"
Enter password:
--------------
mysql  Ver 15.1 Distrib 5.5.56-MariaDB, for Linux (x86_64) using readline 5.1

Connection id:          10
Current database:       hive
Current user:           hive@ip-172-31-7-188.ap-southeast-1.compute.internal
SSL:                    Not in use
Current pager:          stdout
Using outfile:          ''
Using delimiter:        ;
Server:                 MariaDB
Server version:         5.5.56-MariaDB MariaDB Server
Protocol version:       10
Connection:             ip-172-31-7-188.ap-southeast-1.compute.internal via TCP/IP
Server characterset:    latin1
Db     characterset:    utf8
Client characterset:    utf8
Conn.  characterset:    utf8
TCP port:               3306
Uptime:                 39 min 47 sec

Threads: 1  Questions: 37  Slow queries: 0  Opens: 0  Flush tables: 2  Open tables: 26  Queries per second avg: 0.015
--------------

[root@ip-172-31-7-188 centos]# mysql -h ip-172-31-7-188.ap-southeast-1.compute.internal -u hive -p hive -e "show databases;"
Enter password:
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| test               |
+--------------------+


[root@ip-172-31-7-188 centos]# mysql -h ip-172-31-7-188.ap-southeast-1.compute.internal -u scm -p scm -e "status;"                                                                           Enter password:
--------------
mysql  Ver 15.1 Distrib 5.5.56-MariaDB, for Linux (x86_64) using readline 5.1

Connection id:          12
Current database:       scm
Current user:           scm@ip-172-31-7-188.ap-southeast-1.compute.internal
SSL:                    Not in use
Current pager:          stdout
Using outfile:          ''
Using delimiter:        ;
Server:                 MariaDB
Server version:         5.5.56-MariaDB MariaDB Server
Protocol version:       10
Connection:             ip-172-31-7-188.ap-southeast-1.compute.internal via TCP/IP
Server characterset:    latin1
Db     characterset:    utf8
Client characterset:    utf8
Conn.  characterset:    utf8
TCP port:               3306
Uptime:                 43 min 4 sec

Threads: 1  Questions: 44  Slow queries: 0  Opens: 0  Flush tables: 2  Open tables: 26  Queries per second avg: 0.017
--------------



[root@ip-172-31-7-188 centos]# mysql -h ip-172-31-7-188.ap-southeast-1.compute.internal -u scm -p scm -e "show databases;"
Enter password:
+--------------------+
| Database           |
+--------------------+
| information_schema |
| scm                |
| test               |
+--------------------+

