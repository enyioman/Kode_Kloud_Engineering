1. SSH into Backup Server:

```
ssh clint@stbkp01
sudo su -
```

2. Replace string using Linus `sed` command:

```
sed -i 's/Text/LUSV/g' /root/nautilus.xml
```

