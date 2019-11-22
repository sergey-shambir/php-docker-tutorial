# Создание проекта Symfony 4 и Docker-контейнера для него

>Инструкция основана на [Installing & Setting up the Symfony Framework](https://symfony.com/doc/current/setup.html) и адаптирована для Docker

## Подготовка Docker-контейнера

Согласно [документации](https://symfony.com/doc/current/setup.html), для работы с Symfony 4 нужны

* PHP 7.2 и выше с расширениями, которые уже есть в готовом образе `php:7.3-fpm` из Docker Hub
* Composer
* установленный дистрибутив Symfony

Для установки Composer мы взяли скрипт из инструкции [How do I install Composer programmatically?](https://getcomposer.org/doc/faqs/how-to-install-composer-programmatically.md).
Для установки Symfony мы используем `wget https://get.symfony.com/cli/installer -O - | bash` согласно документации

Сделайте следующее:
1. Клонируйте себе этот репозиторий: `git clone https://github.com/sergey-shambir/php-docker-tutorial`
2. Затем перейдите в каталог клона: `cd php-docker-tutorial`
3. Чтобы собрать образ для работы с Symfony, запустите `docker build -t symfony:dev 02_symfony/docker-symfony/`
    * после этого у вас появится docker-образ с именем `"symfony:dev"`, в котором есть PHP, composer и symfony

При желании вы можете скопировать в свой проект каталог `docker-symfony` вместе с Dockerfile и скриптами.

## Создание проекта

Для запуска symfony из контейнера мы будем использовать скрипт `02_symfony/bin/symfony`, который запускает образ `symfony:dev`


TODO
TODO
TODO
TODO
TODO
