1. SSH into App Server 1

```
ssh tony@stapp01
```

2. Login as root

```
sudo su -
```

3. Create user `john` without a home directory

```
useradd --no-create-home john
```

