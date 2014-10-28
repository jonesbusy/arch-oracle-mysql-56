arch-oracle-mysql-56
====================

Oracle MySQL 5.6 package for Arch Linux.

# Installation

```$ makepkg -i```

It will build and install the following package `oracle-mysql-5.6.21-1`

# Usage

Start the service and connect to the MySQL server

```
$ systemctl start oracle-mysql.service
$ /usr/local/mysql/bin/mysql --defaults-file=/usr/local/mysql/my.cnf
```

# Package tree

__Installation folder__

`/opt/oracle-mysql`

with symlink to 

`/usr/local/mysql`

__Service file__

`/usr/lib/systemd/system/oracle-mysql.service`

__PID__

`/var/run/oracle-mysql/oracle-mysql.pid`

__Socket__

`/var/run/oracle-mysql/oracle-mysql.pid`


# Contributing

* [Fork](https://help.github.com/articles/fork-a-repo)
* Create a feature branch - `git checkout -b feature`
* Push to your branch - `git push origin feature`
* Create a [pull request](http://help.github.com/pull-requests/) from your branch

# License

__arch-oracle-mysql-56__ is licensed under the GPLv2 License. See [LICENSE.txt](https://github.com/jonesbusy/arch-oracle-mysql-56/blob/master/LICENSE) for the full text.