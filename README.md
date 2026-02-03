# cloudflared + watchtower

Runs Cloudflare Tunnel in Docker with auto-updates.

## Setup

1. Get token from https://dash.cloudflare.com/
2. Put it in docker-compose.yml
3. `docker compose up -d`

That's it.

## What it does

- Runs cloudflared (limited to 128MB RAM, 10% CPU)
- Watchtower updates it daily
- Both restart on crash

## Commands

```bash
docker compose up -d         # start
docker compose logs -f       # logs
docker compose down          # stop
