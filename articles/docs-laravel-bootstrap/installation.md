## Instalation of Laravel

Laravel can be installed using three methods.

- Laravel Installer
- Composer
- Direct Download

The fastest method is using the Laravel Installer.

### Laravel installer

You can use the Laravel installer PHAR archive to create new laravel projects from the command line. You'll need to download the file and move it into /usr/local/bin.
This can be done by using the following command.

```
curl -O http://laravel.com/laravel.phar && mv laravel.phar /usr/local/bin/laravel && chmod +x /usr/local/bin/laravel
```

If successfull you should now be able type `laravel` at the command line to see a list of available options. Creating a new laravel app is then as simple as running

```
laravel new my-project
```


### Composer installation

If you have [composer](http://getcomposer.org/) installed globall on your machine you can create a new laravel project using the following command

```
composer create-project laravel/laravel --prefer-dist my-project
```

This will install laravel and download it's dependencies in a new directory called `my-project`


