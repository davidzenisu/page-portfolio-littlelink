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