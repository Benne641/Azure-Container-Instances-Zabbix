# Azure-Container-Instances-Zabbix
Work project to run zabbix on Azure ACI with Azure Managed SQL instances

- 11/13/20
Initial yaml deployment 
    - creates a container group with zabbix server and zabbix web frontend
    - passes enviroment variables with secure flag to not allow browsing in azure
    - containers are linked to managed mysql DB 8.0 in azure 
    - you will need to add the users and grant privileges on the mysql server 
          mysql -u 'azadmin@dep-admysql1' -p -h <ip / host name here> -P 3306;