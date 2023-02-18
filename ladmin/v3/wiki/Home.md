**[L-Admin](https://github.com/hexters/ladmin)** is a Laravel administration package that allows web developers to quickly create an admin panel for their website. The package includes features such as user management, access control management, task management, file management, email management, and many more. The package is designed to save time and effort in building an admin panel and allows developers to focus on building the core features of their web application.

# 🚀 Quickstart

Follow the steps below to get started faster! Add the repository by running the command below.

```bash
composer require hexters/ladmin
```

Follow the installation to start build awesome apps.
```bash
php artisan ladmin:install --and=ladmin:setup
```

Run migrate and seed, to install ladmin database tables
```bash
php artisan migrate --seed
```

Installation is complete, please access `http://localhost:8000/administrator`

![Login Page](https://raw.githubusercontent.com/hexters/assets/main/ladmin/v3/captures/login-page.png)


# Customization Color and Assets

To change the ladmin style, you just need to run `Vite`, before that you should install nodejs modules in `Modules/Ladmin` folder. Follow this steps below.

```bash

// Install node modules 

cd Modules/Ladmin && npm install

// Go back to directory root project and run vitejs

npm run dev

```
You can start changing javascript and css.
