# [Phinx](https://phinx.org): Simple PHP Database Migrations

[![Build Status](https://github.com/cakephp/phinx/workflows/Phinx%20CI/badge.svg?branch=master&event=push)](https://github.com/cakephp/phinx/actions?query=workflow%3A%22Phinx+CI%22+branch%3Amaster+event%3Apush)
[![Build Status](https://img.shields.io/travis/com/cakephp/phinx?style=flat-square)](https://travis-ci.com/cakephp/phinx)
[![Build status](https://ci.appveyor.com/api/projects/status/9vag4892hfq6effr)](https://ci.appveyor.com/project/robmorgan/phinx)
[![Code Coverage](https://img.shields.io/coveralls/cakephp/phinx/master.svg?style=flat-square)](https://coveralls.io/r/cakephp/phinx?branch=master)
[![Latest Stable Version](https://poser.pugx.org/robmorgan/phinx/version.png)](https://packagist.org/packages/robmorgan/phinx)
[![Minimum PHP Version](https://img.shields.io/badge/php-%3E%3D%207.2-8892BF.svg)](https://php.net/)
[![Total Downloads](https://poser.pugx.org/robmorgan/phinx/d/total.png)](https://packagist.org/packages/robmorgan/phinx)
[![Join the chat at https://gitter.im/phinx-php/Lobby](https://badges.gitter.im/phinx-php/Lobby.svg)](https://gitter.im/phinx-php/Lobby)

## Intro

Phinx makes it ridiculously easy to manage the database migrations for your PHP app. In less than 5 minutes, you can install Phinx and create your first database migration. Phinx is just about migrations without all the bloat of a database ORM system or framework.

**Check out [book.cakephp.org/phinx](https://book.cakephp.org/phinx) ([EN](https://book.cakephp.org/phinx), [ZH](https://tsy12321.gitbooks.io/phinx-doc/)) for the comprehensive documentation.**

![phinxterm](https://cloud.githubusercontent.com/assets/178939/3887559/e6b5e524-21f2-11e4-8256-0ba6040725fc.gif)

### Features

* Write database migrations using database agnostic PHP code.
* Migrate up and down.
* Migrate on deployment.
* Seed data after database creation.
* Get going in less than 5 minutes.
* Stop worrying about the state of your database.
* Take advantage of SCM features such as branching.
* Integrate with any app.

### Supported Adapters

Phinx natively supports the following database adapters:

* MySQL
* PostgreSQL
* SQLite
* Microsoft SQL Server

## Install & Run

See [version and branch overview](https://github.com/cakephp/phinx/wiki#version-and-branch-overview) for branch and PHP compatibility.

### Composer

The fastest way to install Phinx is to add it to your project using Composer (https://getcomposer.org/).

1. Install Composer:

    ```
    curl -sS https://getcomposer.org/installer | php
    ```

1. Require Phinx as a dependency using Composer:

    ```
    php composer.phar require robmorgan/phinx
    ```

1. Install Phinx:

    ```
    php composer.phar install
    ```

1. Execute Phinx:

    ```
    php vendor/bin/phinx
    ```

### As a Phar

You can also use the Box application to build Phinx as a Phar archive (https://box-project.github.io/box2/).

1. Clone Phinx from GitHub

    ```
    git clone https://github.com/cakephp/phinx.git
    cd phinx
    ```

1. Install Composer

    ```
    curl -s https://getcomposer.org/installer | php
    ```

1. Install the Phinx dependencies

    ```
    php composer.phar install
    ```

1. Install Box:

    ```
    curl -LSs https://box-project.github.io/box2/installer.php | php
    ```

1. Create a Phar archive

    ```
    php box.phar build
    ```

## Documentation

Check out https://book.cakephp.org/phinx for the comprehensive documentation.

Other translations include:

 * [Chinese](https://tsy12321.gitbooks.io/phinx-doc/) (Maintained by [@tsy12321](https://github.com/tsy12321/phinx-doc))

## Contributing

Please read the [CONTRIBUTING](CONTRIBUTING.md) document.

## News & Updates

Follow [@CakePHP](https://twitter.com/cakephp) on Twitter to stay up to date.

## Limitations

### PostgreSQL

- Not able to set a unique constraint on a table (<https://github.com/cakephp/phinx/issues/1026>).


## Misc

### Version History

Please read the [release notes](https://github.com/cakephp/phinx/releases).

### License

(The MIT license)

Copyright (c) 2017 Rob Morgan

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
