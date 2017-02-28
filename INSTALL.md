# WordPress Project Template

## Requirements

* Composer
* NPM
* yarn
* bower
* WP CLI

## Install

```sh
$ # Clone GIT repository
$ git clone https://github.com/horttcore/WordPress-Project-Boilerplate.git WordPress-Project-Boilerplate

$ # Navigate into new directory
$ cd WordPress-Project-Boilerplate

$ # install using composer
$ composer install

$ # Edit enviroments
$ cp wp-config.env.sample.php wp-config.env.php
```

Point root url to `public/index.php`

Set security salts in `wp-config.default.php`

Set table prefix in `wp-config.default.php`

### Development

```sh
$ mv wp-config.development.sample.php wp-config.development.php
```
Edit database connection settings

```sh
$ # Go to theme folder
$ yarn
$ gulp
```

### Staging

```sh
$ # Edit database connection settings
$ mv wp-config.staging.sample.php wp-config.staging.php
```

#### Restrict Access

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

### Production

```sh
$ # Edit database connection settings
$ mv wp-config.production.sample.php wp-config.production.php
```
