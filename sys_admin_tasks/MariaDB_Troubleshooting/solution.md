SSH into server

```
ssh peter@stdb01
```

```
sudo su -
```

Start mariadb service

```
systemctl start mariadb
```

Check complete status of failed mariadb service

```
systemctl status mariadb -l
```


Check the logs

```
cat /var/log/mariadb/mariadb.log
``` 
Check the permissions

```
ll /var/run/mariadb/ -a
```

Change permission to allow all

```
chmod -R 777 /var/run/mariadb
```

Restart mariadb

```
systemctl restart mariadb
```