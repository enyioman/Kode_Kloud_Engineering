1. From the Jump Host server, Secure copy the banner to the /tmp directory of the app server 1 (stapp01). Repeat same on app servers 2 & 3 (stapp02 and stapp03) respectively.
```
scp -r /home/thor/nautilus_banner tony@stapp01:/tmp
scp -r /home/thor/nautilus_banner steve@stapp02:/tmp
scp -r /home/thor/nautilus_banner banner@stapp03:/tmp
```

2. SSH into each server and move the nautilus banner from the /tmp to the /etc/motd directory

```
mv /tmp/nautilus_banner /etc/motd
```


3. For the database server, SSH into the server and install openssh-clients

```
ssh peter@stdb01
sudo su -
yum install -y openssh-clients
```

4. From the jump server, REPEAT STEP1 and STEP2 to transfer the banner to the DB server

5. Log out and log into the respective servers to validate the copied templates.