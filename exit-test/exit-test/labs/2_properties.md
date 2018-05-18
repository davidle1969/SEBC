[root@ip-172-31-7-188 schema]# ./scm_prepare_database.sh mysql -h `hostname -f` scm scm
Enter SCM password:
JAVA_HOME=/usr/java/jdk1.8.0_162
Verifying that we can write to /etc/cloudera-scm-server
Creating SCM configuration file in /etc/cloudera-scm-server
Executing:  /usr/java/jdk1.8.0_162/bin/java -cp /usr/share/java/mysql-connector-java.jar:/us                                                                                                 r/share/java/oracle-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterpris                                                                                                 e.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db.
[                          main] DbCommandExecutor              INFO  Successfully connected                                                                                                  to database.
All done, your SCM database is configured correctly!
