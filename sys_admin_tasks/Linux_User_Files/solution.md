1. SSH into App Server 1

```
ssh tony@stapp01
sudo su -
```

2. Check for files and directories

```
ll /home/usersdata
```

3. Find files owned by user `javed`

```
find /home/usersdata/ -type f -user kirsty |wc -l
```

4. Copy to `/ecommerce` directory while retaining the folder structure

```
find /home/usersdata/ -type f -user javed -exec cp --parents {} /ecommerce \;
```

5. Validate copy by listing the destination directory

```
ll /ecommerce/home/usersdata
```

