1. SSH into App Server 3

```
ssh banner@stapp03
sudo su -   
```

2. Modify the `resolve.conf` file to contain Google DNS IP

```
vi /etc/resolv.conf
```

then add 
```
nameserver 8.8.8.8 or nameserver 8.8.4.4
```

3. Save modification