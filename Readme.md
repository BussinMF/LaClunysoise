# SiteWeb de la Clunysoise

⚙️ Installation
--------------

Install bundles / modules.
```sh
composer install
```
```sh
npm install
```

Compile webpack in real time
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

Controller
```sh
symfony console make:controller
```

Authentication
```sh
symfony console make:user Admin
```

Password Hash
```sh
symfony console security:hash-password
```

SQL Req. to create/set the user
```sh
INSERT INTO admin (id, username, roles, password) 
VALUES (null, 'admin', '["ROLE_ADMIN"]', 
'-- PasswordHash with \ to escape $ --');
```

Auth page creation
```sh
symfony console make:auth
```