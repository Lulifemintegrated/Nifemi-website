# Nifemi Website

A lightweight, dependency-free website served by Node.js.

## Alloy

Start the site with the checked-in Alloy Compose configuration:

```sh
docker compose -f docker-compose.alloy.yaml up -d
```

The application listens on port `3000`. Alloy reads `.alloy/environment.json` and proxies the site through `http://localhost:8080`.

Check the service status and health endpoint with:

```sh
docker compose -f docker-compose.alloy.yaml ps
curl http://localhost:3000/health
```
