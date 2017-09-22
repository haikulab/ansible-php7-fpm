ansible-php7.1-fpm for Debian/Ubuntu
============

Ansible role for installing php-fpm on the your Debian/Ubuntu system.

## php7.1 by default

## Overwrite Default Variables

The `vars/main.yml` file should contain your list of packages you want to install in order to override defaults found in `defaults/main.yml`.

Additionally, you can overwrite the variables as part of your playbook.

```yml
---
...
  vars:
    php_ppa: "ondrej/php"
    php_user: www-data
    php_group: www-data
    php_listen: /var/run/php7.1-fpm.sock
...
```

## Special thanks

Special thanks go to **Mathias Leppich** for [a handy script](https://gist.github.com/muhqu/91497df3a110f594b992) that allows for clearing of Opcache via cli command.
