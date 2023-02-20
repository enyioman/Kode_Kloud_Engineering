1. SSH into App Server 2

```
ssh steve@stapp02
sudo su -
```

2. Update Centos and install NTP

```
yum install update -y @@ yum install -y ntp
```

3. Configure NTP server and add `server 3.pool.ntp.org`

```
vi /etc/ntp.conf
```

