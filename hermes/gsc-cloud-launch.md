# GSC Cloud — Production Launch (2026-08-08)

## Текущее состояние
- server.py: FastAPI, 9 эндпоинтов, готов
- Dockerfile + docker-compose.yml + nginx.conf + index.html: готовы
- Требования: requirements.txt (fastapi, uvicorn, pydantic, stripe)
- Judge: 0.95 ✅
- Тест: curl — 148 находок, express — 52

## Блокер
`server.py` не копируется в Docker-образ (`COPY . /app/` сбоит).
Причина: файл был chmod 600 → `chmod 644 server.py` уже сделано.
Нужно: `DOCKER_BUILDKIT=0 docker build --no-cache .` и проверить что файл в контейнере.

## Что делать дальше
1. chmod 644 ~/gsc/server.py
2. docker rm -f gsc-api && docker rmi -f gsc-api:latest
3. DOCKER_BUILDKIT=0 docker build --no-cache ~/gsc
4. docker run -d --name gsc-api -p 8081:8000 gsc-api
5. curl localhost:8081/health → должно вернуть JSON
6. curl localhost:8081/api/v2/billing/plans → должно вернуть планы

## После запуска
- Создать GitHub App: Settings → Developer settings → GitHub Apps → New
- Получить Client ID + Client Secret
- Stripe: создать аккаунт, получить ключи
- Домен: купить gsc.dev или gsc-security.com
- SSL: certbot для домена

## Дополнительно
- GSC SaaS модель: Free/Pro/Team/Enterprise ($0/$49/$199/$999)
- API ключи: gsk_... через /api/v2/auth/signup
- БД: /data/gsc_cloud.db в Docker volume
