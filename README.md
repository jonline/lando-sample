# Lando

- Install [Docker](https://www.docker.com/products/docker)
- Install [Docker Compose](https://docs.docker.com/compose/install/)
- Install [Lando](http://docs.devwithlando.io/installation/installing.html)
- Identify and stop any local service listening on port 80:
```
$ netstat -lnp | grep 80
```
- Open a terminal window and type the following:
```
$ cd /path/to/project (ie. /var/www)
$ git clone from git repo
$ cd lando-sample
$ wget database
$ lando rebuild -y
$ lando db-import db-sql
$ lando drush uli
```
- Click on the link above to login as user 1 or visit the site at [http://lando-sample.lndo.site](http://lando-sample.lndo.site).

If you want to stop Lando, execute the following:
```
$ lando stop
```
If you want to start Lando, execute the following:
```
$ lando start
```
If you need to reset the login, execute the following:
```
$ lando drush uli
```
If you need to access the container instance for any reason, execute the following:
```
$ lando ssh
```
Read more about [Lando](http://docs.devwithlando.io/).
