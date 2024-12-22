# Symfony API process

# Creating web application and installing dependancies

## Initializing the application

Initializing project
```
composer create-project symfony/skeleton .
git init
```

Dependancies required :
```
composer require api-platform/core
composer require symfony/maker-bundle --dev
```

Creating first controller
```
php bin/console make:controller TestController
```

##Dependancies for Authentification

Google authentification
```
compsoer require google/auth
```
