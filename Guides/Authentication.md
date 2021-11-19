### Authentication

In order to use authentication we need to define the variables in an **.env** file which will be used by masonite to register and authenticate the users.

Let's create our new app.

``` bash
mkdir 2
cd 2
craft new
```

Create our **.env** file. We will use the **sqlite** provider but many others are supported aswell.

``` bash
DB_CONNECTION=sqlite
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=auth.db
DB_USERNAME=root
DB_PASSWORD=root
```

After that issue the **craft auth** and **craft migrate** commands. This will setup the controllers and create the table in the sqlite database that holds our users.