# Resume

A static resume portfolio site for showcasing work experience, selected projects, and technical skills.

## Local Setup

Use Node through `nvm` so local development matches the project baseline:

```sh
brew bundle
nvm use
npm install
```

`Brewfile` installs `nvm`. The project targets Node 24, the current LTS line for this setup.

## Development

```sh
npm run dev
```

This serves the static site from `site/` at `http://127.0.0.1:8000`. Set a different port with:

```sh
PORT=8080 npm run dev
```

## Formatting

```sh
npm run format
npm run format:check
```

`format` updates files with Prettier. `format:check` verifies formatting without changing files.

## Deployment

GitHub Pages is deployed by `.github/workflows/pages.yml`. The workflow publishes the `site/`
directory when changes land on `main`, and it can also be run manually from GitHub Actions.
