## Commandes

- Liste des commandes make
```
symfony console list make
```

- Initialisation projet
```
symfony new my_project_dir --version="6.3.*" -webapp
composer require symfony/webpack-encore-bundle
npm install
composer require symfony/ldap
symfony make:controller Home
```

- Webpack/Encore
```
npm run build
```
- Générer les routes Symfony vers JS
```
php bin/console fos:js-routing:dump --format=json --target=public/js/fos_js_routes.json
```

- Installer pour prod
```
composer install --no-dev --optimize-autoloader
```

- Mettre à jour
```
composer update --with-all-dependencies
```

- Installer assets frontend
```
npm run watch/build
```

- Démarrer le serveur local
```
symfony server:start
```
