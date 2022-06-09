# WordPress Docker-Compose

Стартовый набор для быстрой и комфортной разработки WordPress сайтов с помощью Docker и Docker-Compose.

### Требования

Для работы у вас должны быть установленны последние версии:
* [Docker и Docker Compose](https://www.docker.com/products/docker-desktop)
* [Composer](https://getcomposer.org/download/)

### Установка

1. Клонируйте репозиторий в нужную директорию
    ```bash
    git clone git@github.com:arthursatarov/wordpress-docker-compose
    ```
2. Перейдите в папку созданного проекта и удалите историю разработки
    ```bash
    rm -rf .git
    ```
2. Изменимте настройки Wordpress, MySQL и phpMyAdmin в файле `.env`
3. Добавьте требуемые для установки WordPress плагины и темы в файл `composer.json`
4. Запустите Docker контейнер
    ```bash
    docker-compose up -d
    ```
4. Измените права доступа для редактирования файлов
    ```bash
    sudo chmod 777 -R www
    ```

### Команды
```bash
  docker-compose up -d      # создает и запускает Docker контейнер
  docker-compose down       # останавливает и удаляет Docker контейнер
  composer update           # устанавливает зависимости
```
* [Список команд Docker Compose](https://docs.docker.com/compose/reference/)
* [Список команд Composer](https://getcomposer.org/doc/03-cli.md)
