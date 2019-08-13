# linux-server-config
Linux server configuration for Udacity project.
## Ip Address
3.120.187.24
## SSH port 
2200
## Url
http://3.120.187.24/
## Software installed:
- apache2
- postgresql
- postgresql-contrib
- python-psycopg2
- libpq-dev
- libapache2-mod-wsgi-py3
- python-dev

#### item-catalog clone
On the project's venv:
 - psycopg2
 - flask
 - flask-login
 - flask-dance
 - ...

## Configuration:
1. Added grader user with sudo access.
2. Disabled ssh logging for the root user.
3. Changed ssh port to 2200.
4. Disabled password authentiaction.
5. Configured UFW firewall to accept only on 22, 2200 (ssh), 80 (tcp), 123 (ntp).
6. Configured apache to serve item-catalog app (/etc/apache2/sites-available/item-catalog.conf file)

## Third-party resources:
https://www.codementor.io/abhishake/minimal-apache-configuration-for-deploying-a-flask-app-ubuntu-18-04-phu50a7ft
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-18-04
https://docs.sqlalchemy.org/en/13/dialects/postgresql.html#module-sqlalchemy.dialects.postgresql.psycopg2
https://pypi.org/project/psycopg2/
https://www.techiediaries.com/error-you-need-to-install-postgresql-server-dev-x-y-for-building-a-server-side-extension-or-libpq-dev-for-building-a-client-side-application/
