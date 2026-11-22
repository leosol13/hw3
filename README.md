## Шаблон для третьего ДЗ по ИПР
Docker compose
Переменные
`HOST_PORT` (`8080`)
`PORT` (`8000`)
`GREETING`
`STORAGE` (`sqlite`)
`DATA_FILE` (`/data/counter.db`)
Команды
cp .env.example .env
docker compose up -d --build
Проверка сохранения счётчика:
curl -s [http://127.0.0.1:8080/](http://127.0.0.1:8080/)
curl -s -X POST [http://127.0.0.1:8080/increment](http://127.0.0.1:8080/increment)
docker compose down
docker compose up -d
curl -s [http://127.0.0.1:8080/](http://127.0.0.1:8080/)
Логи и остановка:
docker compose logs -f
docker compose down
