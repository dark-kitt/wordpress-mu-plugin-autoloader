# **WordPress MU-Plugin Autoloader**

Project: [Part 1](https://github.com/dark-kitt/wordpress-boilerplate/tree/main), [**Part 2**](https://github.com/dark-kitt/wordpress-theme-configuration), [Part 3](https://github.com/dark-kitt/wordpress-theme-vue)

---

## Introduction

This WordPress MU-Plugin loads MU-Plugins from **subdirectories**. WordPress only looks for PHP files right inside the MU-Plugins directory, and not for files in subdirectories (unlike for normal plugins).

After installing the package, copy the ***mu-plugin-autoloader.php*** file inside of the MU-Plugins directory (*`/mu-plugins`*), to load WordPress MU-Plugins automatically.

This MU-Plugin is a modified version based on the [richardtape/subdir-loader.php](https://gist.github.com/richardtape/05c70849e949a5017147) Github Gist.

### Requirements

* [PHP: ^7.*](https://www.php.net/manual/de/mysql-xdevapi.installation.php)
* [WordPress: ^5.*](https://wordpress.org/support/article/how-to-install-wordpress/)

## Installation

```shell
composer require dark-kitt/wordpress-mu-plugin-autoloader
```

Note, for a specific commit of your VCS Repo `"require": { "vendor/repo_name": "dev-main#eec8698" }` (branch#commit).

**common composer cmds**

```shell
composer install
composer update
# package control
composer require verdor/package
composer remove verdor/package

composer clear-cache
composer show -i # installed packages
```

---
---

## License

[![](https://upload.wikimedia.org/wikipedia/commons/e/e5/CC_BY-SA_icon.svg)](https://creativecommons.org/licenses/by-sa/4.0)

---

## Includes

* [richardtape/subdir-loader.php](https://gist.github.com/richardtape/05c70849e949a5017147)