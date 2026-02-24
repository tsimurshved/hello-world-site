# Hello World Site

Minimal HTML starter project with separate staging and production deployments.

## URLs

- Production: https://hello.ragaihub.com
- Staging: https://hello-staging.ragaihub.com

## Branch Flow

- `staging` branch -> staging environment
- `main` branch -> production environment

## Deployment

A GitHub Actions workflow deploys automatically on push:

- push to `staging` runs `/opt/hello-world-site/scripts/deploy-staging.sh` on the VPS
- push to `main` runs `/opt/hello-world-site/scripts/deploy-production.sh` on the VPS
