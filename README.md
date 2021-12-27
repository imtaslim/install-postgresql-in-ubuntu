# install-postgresql-in-ubuntu
PostgreSQL, or Postgres, is a relational database management system that provides an implementation of the SQL querying language. It’s standards-compliant and has many advanced features like reliable transactions and concurrency without read locks.

# Update
~~~
sudo apt-get update
~~~

# Install the package
~~~
sudo apt install postgresql postgresql-contrib
~~~

# Configure user
~~~
sudo -i -u postgres
~~~

# access the Postgres prompt
~~~
psql
~~~

# Password initialisation
~~~
alter user postgres with password 'your_password'
~~~

# for exit the psql server
~~~
\q
~~~
then
~~~
exit;
~~~

# for creating new user
~~~
sudo -u postgres createuser --interactive
~~~

now set name and confirm this
~~~
Output
Enter name of role to add: sammy
Shall the new role be a superuser? (y/n) y
~~~

Once logged in, you can get check your current connection information by running:
~~~
\conninfo
~~~

you can go to this link for more information
https://www.digitalocean.com/community/tutorials/how-to-install-postgresql-on-ubuntu-20-04-quickstart
