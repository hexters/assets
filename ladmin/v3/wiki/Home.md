# 🚀 Quickstart

Follow the steps below to get started faster! Add the repository by running the command below.

```bash
$ composer require hexters/ladmin
```

Follow the installation with the `--with-admin-table` option.
```
$ php artisan ladmin:install --with-admin-table
```

Run migrate and seed, to install ladmin database tables
```bash
$ php artisan migrate --seed
```

And run seeder ladmin module, to assign role and permission to existing user.
```bash
$ php artisan module:seed Ladmin
```

Installation is complete, please access `http://localhost:8000/administrator`

![Login Page](https://github.com/hexters/assets/blob/main/ladmin/v2/captures/login-page.png?raw=true)

# 🧰 Manual Installation

If you want to use the `App\Models\User` model class as a login account, then follow the steps below.

Use `\Hexters\Ladmin\LadminAccount` into model `\App\Modules\User` see the example.
```php
. . .
use Hexters\Ladmin\LadminAccount;

class User extends Authenticatable {

  use HasApiTokens, HasFactory, Notifiable, LadminAccount;

  . . .
```

Open file `\Database\Seeders\DatabaseSeeder`, add the code below or you can create your own seeder file.
```php

\App\Models\User::factory(10)->create();

```

Follow the installation below.

```
$ php artisan ladmin:install
```

Run migrate and seed, to install ladmin database tables
```bash
$ php artisan migrate --seed
```

And run seeder ladmin module, to assign role and permission to existing user.
```bash
$ php artisan module:seed Ladmin
```

And please access `http://localhost:8000/administrator`