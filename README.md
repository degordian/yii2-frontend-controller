Yii2 Frontend Controller
========================
A special controller for your frontend department that allows for easy access to any view/layout combination without going through their respective controllers (avoiding the need to login or have a db).

Installation
------------

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require --prefer-dist degordian/yii2-frontend-controller "*"
```

or add

```
"degordian/yii2-frontend-controller": "*"
```

to the require section of your `composer.json` file.


Usage
-----

To access the module, you need to add this to your application configuration:
```php
<?php
    ......
    'modules' => [
        'frontend' => [
            'class' => 'degordian\frontendController\Module',
        ],
    ],
    ......
```

`Then to use this extension open up http://your-project.local/frontend/<layout>/<controller>/<action>`

Advanced usage allows for a custom output message or dynamic number of iterations by appending ?m=<integer>&i=<message>
example:

`http://my-project.local/frontned/main/site/index?m=Short+message&i=15`
