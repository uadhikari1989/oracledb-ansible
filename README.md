# oracledb-ansible
Ansible playbook to configure a CentOS/RHEL/Oracle Linux 7 server with Oracle 12c R1 Enterprise Edition Database

Requirement : 

- Ansible
- Centos 7 as a deployment server (also the server might need about 30gb space and about 2-3 gb RAM. )


Download from Oracle support the Oracle installation files: 
- linuxamd64_12102_database_1of2.zip
- linuxamd64_12102_database_1of2.zip
and put them to folder roles/oracle-install/files inside checkout folder

Once the file has been kept in respective folder . Run the following command from Ansible master . 

```
ansible-playbook -i hosts playbook.yml -K

```

After a few minutes a virtual centos machine  with Oracle Database will be ready for you without any further configuration. You can access the Enterprise Manager 

https://x.x.x.x:5500/em

```
username: sys
password: oracle
```


password for Oracle Operating system user is welcome1


