#Categories Management Yii2 Module
Complete category management module for Yii2 based web application, Ready to integrate

* Easy to install
* Create Unlimited Multilevel categories
* Category tree structure to visualize category depth
* Category Image
* Category SEO Meta (Title, keywords, Description)

### 1. Download

Yii2-categories can be installed using composer. Run following command to download and
install Yii2-categories:

```bash
composer require "yiimodules/yii2-categories:dev-master"
```

### 2. Configure

Add following lines to your main configuration file to access this module via web URL:
> **NOTE:** Along with category module you also need to configure redactor Module which installed as dependency in category module as below.

```php
'modules' => [
	'redactor' => 'yii\redactor\RedactorModule',
    'categories' => [
        'class' => 'yiimodules\categories\Module',
    ],
],
```

### 3. Update database schema

The last thing you need to do is updating your database schema by applying the
migrations. Make sure that you have properly configured `db` application component
and run the following command:

```bash
$ php yii migrate/up --migrationPath=@vendor/yiimodules/yii2-categories/migrations
```

## Run module?

```bash
$ http://localhost/YOUR-PROJECT-NAME/web/index.php?r=categories
```