User registration project (no api)
=============
User registration to database via registration form and printout all users to list


## Requirements:
- Composer
- MySQL/MariaDB 
- Symfony (downloadable from: http://symfony.com/download)
- web browser

## Install:

If needed:
```
composer require symfony/runtime
```

Start your MySQL/MariaDB, and then run this in command line:
```
php bin/console doctrine:database:create
```

Database 'example' is now created! Now, migrate table schema to 'example' DB and create table:
```
php bin/console doctrine:migrations:migrate
```

Finally, start server with this command:
```
symfony server:start --no-tls
```

If All done, project is available on:
```
http://localhost:8000/user
```
