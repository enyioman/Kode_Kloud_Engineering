1. We'll first check if ssh key already exists:

```
ls -al ~/.ssh/id_*.pub
```


2. If not present, Create a new ssh key

```
ssh-keygen -t rsa 
```

3. Upload Public Key to remote server to ensure password less connectivity

ssh-copy-id [remote_user]@[server_ip_address] in our case, we are to do this for all app servers in the nautilus datacenter

```
ssh-copy-id tony@stapp01
ssh-copy-id steve@stapp02
ssh-copy-id banner@stapp03
```

4. SSH into one of the appserver to test password-less ssh connectivity

```
ssh tony@stapp01
```