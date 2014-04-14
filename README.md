# Ansible PHP-FPM
Install PHP-FPM 5.4 on Centos/Red Hat/Fedora with Ansible

## Installation
- Clone this repository inside your ```roles``` direcotry
or add as submodule: `git submodule add git@github.com:Vinelab/ansible-php-fpm roles/php-fpm`

- In your playbook:

```yaml
roles:
  - php-fpm
```

## Synopsis
will install the listed services from [remi repo](http://rpms.famillecollet.com):

```yaml
- php
- php-fpm
- php-mbstring
- php-mcrypt
- php-pdo
- php-mysql
- php-xml
- php-gd
```

## Usage

In case you wanted PHP to be setup for development use, i.e. displaying errors, add the following:

```yaml
vars:
  env: development # or any value other than 'production'
```
