## Описание

Это проект Django REST API для управления складами и запасами.

## Установка и запуск

### Предварительные требования

- Установлен Docker и Docker Compose.

### Сборка и запуск контейнера

1. Склонируйте репозиторий:
   git clone <URL>
   cd stocks_products

2. Соберите образ и запустите контейнер:
    docker image build . --tag=stock_product:0.1
    docker run -d -p 8000:8000 <container_id>
    
3. Примените миграции (если не было сделано в Dockerfile):
    docker exec -it <container_id> python manage.py migrate


4. Откройте браузер и перейдите по адресу (http://localhost:8000).

## Закрытие контейнера

Для остановки контейнера используйте:
    docker stop <container_id>

   

