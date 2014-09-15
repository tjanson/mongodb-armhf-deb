mongodb-armhf-deb
=================

MongoDB 2.1.1 package for Raspberry Pi (`armhf`).

Compiled from [RickP/mongopi](https://github.com/RickP/mongopi) with Linaro/Raspbian toolchain.

Packaged with `init` and `conf` files for Raspbian based on [Debian](http://sources.debian.net/src/mongodb/1:2.4.10-2/debian/), using [fpm](https://github.com/jordansissel/fpm).

Download & Installation
-----------------------

Download the [`monogdb_2.1.1_armhf.deb` package](https://github.com/tjanson/mongodb-armhf-deb/raw/release/mongodb_2.1.1_armhf.deb) from [`release`](https://github.com/tjanson/mongodb-armhf-deb/tree/release) branch:

> ```wget https://github.com/tjanson/mongodb-armhf-deb/raw/release/mongodb_2.1.1_armhf.deb```

Install:

> ```sudo dpkg -i mongodb_2.1.1_armhf.deb```

Start service:

> ```sudo /etc/init.d/mongodb start```

Issues? Check `/var/log/mongodb/mongodb.log` and file a bug.

Package it yourself
-------------------

Alternatively, you can take a look at the files in the `master` branch and make modifications.
Then, create the `.deb` with `sh fpmcmd` (requires [fpm](https://github.com/jordansissel/fpm)).

It would probably be easy to adapt this for `rpm` or other systems, if you’re so inclined.

Disclaimer
----------

The code from which these binaries are compiled is very outdated (last commit in 2012). As a consequence, it is quite likely that there are security flaws. It’s definitely not suited for production.
