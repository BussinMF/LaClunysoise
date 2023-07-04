# SiteWeb de la Clunysoise

⚙️ Installation
--------------

Install the PHP dependencies and JS dependencies.
```sh
composer install
```

Install modules
```sh
npm install
```

Compile Webpack in real time
```sh
npm run watch
```

Entities / Database
```sh
symfony console doctrine:database:create
```
```sh
symfony console make:entity
```
```sh
symfony console make:migration
```
```sh
symfony console doctrine:migrations:migrate
```
```sh
symfony console doctrine:schema:update --force
```

Controller
```sh
symfony console make:controller
```

Admin sql
```sh
INSERT INTO admin (id, username, roles, password) 
VALUES (null, 'admin', '["ROLE_ADMIN"]', 
'-- PasswordHash with \ to escape $ --');
```