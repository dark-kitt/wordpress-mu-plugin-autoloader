# **WordPress MU-Plugin Autoloader**
---

## Introduction

This WordPress MU-Plugin loads MU-Plugins from **subdirectories**. WordPress only looks for PHP files right inside the MU-Plugins directory, and not for files in subdirectories (unlike for normal plugins).

After **composer update** copy the ***mu-plugin-autoloader.php*** file inside of the MU-Plugins directory (*`/mu-plugins`*), to load WordPress MU-Plugins automatically.

This MU-Plugin is a modified version based on the [richardtape/subdir-loader.php](https://gist.github.com/richardtape/05c70849e949a5017147) Github Gist.

### Requirements

* [PHP: ^7.*](https://www.php.net/manual/de/mysql-xdevapi.installation.php)
* [WordPress: ^5.*](https://wordpress.org/support/article/how-to-install-wordpress/)

## Installation

Edit your composer.json file and insert the following lines to install the **WordPress MU-Plugin Autoloader**. Run **composer update** and copy the ***mu-plugin-autoloader.php*** file inside of the MU-Plugins directory (*`web/app/mu-plugins`*).
```json
...
"repositories": [{
        "type": "vcs",
        "url": "#"
    }
]
...
"require": {
    "dark-kitt/wordpress-mu-plugin-autoloader": "dev-main"
}
...
```

* copy the code inside of **composer.json**
* run **composer update**

Note, for a specific commit of your VCS Repo `"require": { "vendor/repo_name": "dev-main#eec8698" }` (branch#commit).

**composer cmds**
```text
composer install
composer update

composer clear-cache
composer show -i (installed packages)
```

---
---

## License

[![](https://upload.wikimedia.org/wikipedia/commons/e/e5/CC_BY-SA_icon.svg)](https://creativecommons.org/licenses/by-sa/4.0)

---

## Includes

* [richardtape/subdir-loader.php](https://gist.github.com/richardtape/05c70849e949a5017147)