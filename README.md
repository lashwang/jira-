Create and configure the MySQL database


CREATE DATABASE jiradb CHARACTER SET utf8 COLLATE utf8_bin;
GRANT SELECT,INSERT,UPDATE,DELETE,CREATE,DROP,ALTER,INDEX on jiradb.* TO jirauser@localhost IDENTIFIED BY 'jira';
flush privileges;
SHOW GRANTS FOR jirauser@localhost;

