# Personal Portfolio

A simple, self-hosted link page with branded button styles, powered by (forked from) [LittleLink](https://github.com/sethcottle/littlelink).

## Getting Started

Edit `index.html` to add profile details and links. Themes are controlled by the class on the `html` element, and button styles live in `css/brands.css`.

## Local Development

No build step is required. Open `index.html` directly, or run the included Docker setup:

```bash
docker compose -f docker/compose.yaml up
```

The site will be available at http://localhost:8080.

For Docker configuration details, see [docker/README.md](docker/README.md).

## GitHub Actions Deployment

The Azure Static Web Apps workflow deploys changes to `main` from the `.website` directory. Add these repository secrets in **Settings > Secrets and variables > Actions**:

| Secret | Description |
| --- | --- |
| `AZURE_CLIENT_ID` | Microsoft Entra application (service principal) client ID used by `azure/login` |
| `AZURE_TENANT_ID` | Microsoft Entra tenant ID |
| `AZURE_SUBSCRIPTION_ID` | Azure subscription ID containing the Static Web App |
| `AZURE_SWA_NAME` | Name of the Azure Static Web App |

`GITHUB_TOKEN` is provided automatically by GitHub Actions and does not need to be added manually.