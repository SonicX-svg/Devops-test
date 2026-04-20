# DevOps Test

## Запуск

docker-compose up --build

## Проверка

curl http://localhost

Ожидаемый ответ:
Hello from Effective Mobile!

## Архитектура

client → nginx → backend

- nginx принимает HTTP-запросы на 80 порту
- проксирует их в backend
- backend — простой HTTP сервер на Python
