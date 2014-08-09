Imagemanager
=================

Manager for images


## Installation

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
$ php composer.phar require amavis442/yii2-imagemanager "dev-master"
```

or add

```
"amavis442/yii2-imagemanager": "dev-master"
```

to the require section of your `composer.json` file.

## Usage

Once the extension is installed, modify your application configuration to include:

```php
return [
	'modules' => [
	    ...
	        'imageManager' => [
	            'class' => 'amavis442\imagemanager\Module',
	            'layout' => '//homepage', // Layout when not logged in yet
	        ],
	    ...
	],
	...
];
```

And run migrations:

```bash
$ php yii migrate/up --migrationPath=@imageManager/migrations
```

## License

imageManager module is released under the MIT License. See the bundled `LICENSE.md` for details.

#INSTALLATION

./yii migrate/up --migrationPath=@imageManager/migrations