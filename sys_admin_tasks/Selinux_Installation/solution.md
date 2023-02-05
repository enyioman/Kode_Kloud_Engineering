1. SSH into Server 1:

```
ssh tony@stapp01
```

2. Check server distribution:

```
cat /etc/os-release
```

3. Install Selinux:

```
sudo yum -y install selinux
```

4. Check Selinux Status:

```
sestatus
```

5. Check and edit Selinux status from `enforcing` to `disabled`:

```
cat /etc/selinux/config | grep SELINUX

sudo vi /etc/selinux/config
```

6. Validate Selinux status one more time:

``` 
sestatus
```