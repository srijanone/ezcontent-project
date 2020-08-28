This is a Composer-based installer for the 
[EZContent](https://www.drupal.org/project/ezcontent) Drupal distribution.

## Getting Started with Drupal 8 Installation

EzContent can be installed in two ways:

1. Via Drupal Composer

 * Choose a name for your project, like “MY_PROJECT”
 * Use the given command to create the project
 * The command will download Drupal core along with necessary modules,
Ez content profile, and all other dependencies necessary for the project
```bash
composer create-project srijanone/ezcontent-project:1.0 MY_PROJECT --no-interaction
```

Note: In case you come across any memory issues, run this command -
```bash
php -d memory_limit=-1 /path/to/composer.phar create-project
srijanone/ezcontent-project:1.0 MY_PROJECT --no-interaction
```

2. Via Acquia BLT

To create a new Acquia BLT project using Ez content, use the following commands
```bash
composer create-project --no-interaction acquia/blt-project MY_PROJECT;
cd MY_PROJECT;
composer require srijanone/ezcontent:^1.0;
```
Warning: There may be updates to BLT, Lightning which may break the setup. If
you see any issue, please open a new issue in the issue queue.

## Getting Started with Drupal 9 Installation

1. Via Drupal Composer

```bash
composer create-project srijanone/ezcontent-project:9.x-dev
MY_PROJECT --no-interaction
```
2. Via Acquia BLT

```bash
composer create-project --no-interaction acquia/drupal-recommended-project
MY_PROJECT;
cd MY_PROJECT;
composer require srijanone/ezcontent:9.x-dev;
```

By using these commands you will get a EZContent site as your final output.
Login to your site using your database and webserver. Composer will install
all the required dependency into vendor folder. Always remember composer.json
and composer.lock files that exist they are controlling your dependencies.

## Docksal Support
This project installer has [Docksal](https://docksal.io/) support.
