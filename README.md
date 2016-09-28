# WordPress Project Template

## Requirements

* Composer
* NPM
* WP CLI

## Install

```sh
$ # Clone GIT repository
$ git clone https://github.com/horttcore/WordPress-Project-Boilerplate.git WordPress-Project-Boilerplate

$ # Navigate into new directory
$ cd WordPress-Project-Boilerplate

$ # install using composer
$ composer install
```

Point root url to `public/index.php`

## Develop

cp local-config-sample.php local-config.php

```sh
$ # Go to theme folder
$ sudo npm install
$ gulp
```
## Staging

### Restrict Access

```sh
$ # Generate .htpasswd
$ htpasswd -c {LOGIN}
```

```sh
# BEGIN ACCESS
AuthName "Restricted Area"
AuthType Basic
AuthUserFile /var/www/domain.com/htdocs/.htpasswd
AuthGroupFile /dev/null
require valid-user
# END ACCESS
```
