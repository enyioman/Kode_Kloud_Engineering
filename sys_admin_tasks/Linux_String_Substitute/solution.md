1. SSH into the App Server 2

```
ssh steve@stapp02
sudo su -
```

2. Search for the word to be deleted

```
cat /home/BSD_DELETE.txt | grep copyright
```

3. Delete the word and save the output in another file

```
sed '/\<copyright\>/d' /home/BSD.txt > /home/BSD_DELETE.txt
```

4. Replace the given word while making sure no to alter any other word containing the string:

```
sed 's/\bthe\b/their/g' /home/BSD.txt > /home/BSD_REPLACE.txt
```






