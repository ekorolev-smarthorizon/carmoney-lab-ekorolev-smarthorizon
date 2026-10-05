1) Учебный сервис **предварительной оценки заявки на заём под ПТС** (`carmoney-lab`): принимает VIN, год, пробег, оценочную стоимость, сумму и срок, считает LTV и возвращает решение `approve` / `review` / `reject` (README.md:3–7).
2) В Makefile: `make up` (поднять сервис и базу), `make down`, `make test` (PHPUnit), `make lint` (`php -l`), `make seed` (перезалить `db/seed.sql`), `make logs`, `make ps`, `make install`, `make help`; в `docker-compose.yml` сервисы `backend` (php -S на 8080) и `db` (mysql:8.0), поднимаются `docker compose up -d --build`.
3) В папке `backend/src/Domain/` — классы `LtvCalculator.php` и `DecisionEngine.php` считают LTV и возвращают `approve` / `review` / `reject` (`DecisionEngine.php:10–18`).
модель: MiniMax-M3 (stg-proxy/training-2026-09-minimax-m3)

