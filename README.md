## Шаблон для третьего ДЗ по ИПР
<<<<<<< HEAD
4 балла логи:
=======
Логи 4 балла:
>>>>>>> 028bec8 (red)
2026-11-22 19:11:44,323 listening port=8000 storage=sqlite
2026-11-22 19:11:51,446 http 172.17.0.1 "GET / HTTP/1.1" 200 -
2026-11-22 19:12:01,270 http 172.17.0.1 "POST /increment HTTP/1.1" 200 -
2026-11-22 19:12:12,251 http 172.17.0.1 "GET / HTTP/1.1" 200 -
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
