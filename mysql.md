```
https://dbeaver.io/files/dbeaver-ce_latest_amd64.deb
```

```
sudo apt install mysql-server
```

```
sudo netstat -tap | grep mysql
```

查看密码
```
sudo cat /etc/mysql/debian.cnf
```

```
mysql -u debian-sys-maint -p
use mysql;
update user set authentication_string=PASSWORD("root") where user='root';
update user set plugin="mysql_native_password";
flush privileges;
quit;
```

```
/etc/init.d/mysql restart;
```

```
mysql -u debian-sys-maint -p
```


