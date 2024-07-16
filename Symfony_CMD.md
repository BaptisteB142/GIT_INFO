## Commandes

- Liste des commandes make
```
symfony console list make
```

- Initialisation projet
```
symfony new my_project_dir --version="6.3.*" -webapp

Voir WEBPACK/Encore

composer require symfony/ux-chartjs
composer require symfony/ldap

symfony console make:controller Home
```

- Webpack/Encore
```
composer require symfony/webpack-encore-bundle
npm install
npm install sass-loader sass webpack --save-dev
==> uncomment //  .enableSassLoader()

npm install file-loader --save-dev
==> add to webpack.config.js :
.copyFiles({
        from: './assets/images',
        to: 'images/[path][name].[hash:8].[ext]'
    })

npm install --save-dev typescript ts-loader
==> uncomment //   .enableTypeScriptLoader();

npm install bootstrap
npm install chart.js
npm run build
```
- Générer les routes Symfony vers JS

```
see https://github.com/FriendsOfSymfony/FOSJsRoutingBundle/blob/master/Resources/doc/installation.rst
and https://grafikart.fr/forum/33790

composer require friendsofsymfony/jsrouting-bundle
=> expose route
=> enable bundle
=>fos_js_routing.yaml

npm i fos-router
php bin/console fos:js-routing:dump --format=json --target=public/js/fos_js_routes.json
```

- Composer install dependancy for dev
```
composer require --dev symfony/maker-bundle
```
- Composer deploy for prod
```
composer install --no-dev --optimize-autoloader
```

- Composer update
```
composer update --with-all-dependencies
```

- Install frontend assets
```
npm install
npm run watch/build
```

- Local Server
```
symfony server:start
symfony server:stop
```


## Ajout d'extensions PHP

- Se rendre dans le dossier suivant et copier les .dll :
```
C:\xampp\php\ext
=> ex : php_sqlsrv_82_ts_x64.dll
```
- Éditer le fichier php.ini et activer les extensions :
```
C:\xampp\php\php.ini
=> ex : extension=php_sqlsrv_82_ts_x64
```
- Ajouter l'extension intl ( international )
```
C:\xampp\php\php.ini
=> ex : extension=php_intl.dll
```

## MAJ des packages NPM

- Installer globalement le package pour vérifier les versions du package.json
```
npm install -g npm-check-updates
```
- Diagnostiquer
```
ncu
```
- Mettre à jour package.json & package-lock.json
```
ncu -u
npm install
```
