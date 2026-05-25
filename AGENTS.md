# Repository Guidelines

## Project Structure & Module Organization

This repository is a static resume portfolio site deployed with GitHub Pages.

- `site/index.html` is the main page.
- `site/styles/` contains CSS.
- `site/assets/` is reserved for images, icons, PDFs, and downloads.
- `scripts/` contains local development utilities.
- `.github/workflows/` contains deployment automation.

## Build, Test, and Development Commands

Use Node through `nvm`:

```sh
brew bundle
nvm use
npm install
npm run dev
```

- `brew bundle` installs local tooling from `Brewfile`.
- `npm run dev` serves `site/` locally.
- `npm run format` formats project files with Prettier.
- `npm run format:check` verifies formatting for CI-style checks.

## Coding Style & Naming Conventions

Use simple, readable static-site conventions:

- Indent HTML, CSS, JavaScript, Markdown, and YAML with 2 spaces.
- Use lowercase, hyphenated filenames such as `resume-print.css`.
- Use semantic HTML where possible: `main`, `section`, `article`, `header`, and `footer`.
- Keep CSS class names descriptive and hyphenated, for example `.experience-item`.
- Avoid unnecessary dependencies for layout or small interactions.

## Testing Guidelines

There are no automated tests yet. Before submitting changes, run `npm run format:check` and manually check the site in a browser for layout, links, spelling, and print behavior if printable resume output is supported.

If tests are added later, place them in `tests/` and document the runner and command in `README.md`. Name test files after the behavior they cover, for example `print-layout.test.js`.

## Commit & Pull Request Guidelines

The Git history currently contains only `Initial commit`, so no detailed project convention has been established. Use short, imperative commit messages:

- `Add resume homepage`
- `Update work experience copy`
- `Improve print styles`

Pull requests should include a concise description, note any visual changes, and include screenshots for layout or styling updates. Link related issues when applicable.

## Agent-Specific Instructions

Keep changes focused and avoid introducing frameworks or build tools unless the task clearly requires them. Preserve the static-site nature of the repository, update documentation when commands or structure change, and do not overwrite user-authored resume content without explicit direction.
