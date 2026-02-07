# InsightfulBytes Infrastructure

Docker deployment configuration for InsightfulBytes blog.

## Quick Deploy

1. Clone this repo on your server
2. Copy `.env.example` to `.env` and fill in values
3. Run: `docker compose up -d`
4. Create superuser: `docker compose exec backend python manage.py createsuperuser`

## Update Deployment
```bash
docker compose pull
docker compose up -d
```

## View Logs
```bash
docker compose logs -f backend
docker compose logs -f frontend
```