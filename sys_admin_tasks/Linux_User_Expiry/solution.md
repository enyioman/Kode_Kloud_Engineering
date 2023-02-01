1. SSH into App Server 2

```
ssh steve@stapp02
```

2. Add user mark

```
sudo adduser mark
```

3. Add expiry date to the user

```
sudo chage -E 2021-12-07 mark
```

4. Check to confirm through user info

```
sudo chage -l mark
```

![User info](./images/info.png)