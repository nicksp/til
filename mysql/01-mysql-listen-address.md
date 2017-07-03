# Make MySQL listen on other interfaces

If you want to change the default behaviour of MySQL that only listen on localhost (127.0.0.1) and make it available from the outside network, you need to edit file `/etc/mysql/my.cnf` and change the following line `bind-address = 127.0.0.1` to read:

```sh
#bind-address = 127.0.0.1
```

Then restart the server:

```sh
sudo service mysql restart
```
