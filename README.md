# PESU Decoded

Welcome to PESUfy — the student-facing site built with Hugo.

This repository contains the Hugo site sources and content for PESUfy.

## About PESUfy

PESUfy is a community-driven resource for PES University students and newcomers. It collects campus guides, department/branch pages, club information, event updates, and helpful how-tos (admissions, hostel, academics). The site aims to:

- Provide clear, student-focused documentation and quick links for campus services.
- Showcase clubs, events, and student projects to encourage participation.
- Offer an easy-to-edit content structure so students and maintainers can contribute.

---

## Quick links

- Config: [hugo.yaml](hugo.yaml#L1-L200)
- Theme / module: [go.mod](go.mod#L1-L200)
- Content: [content/](content/_index.md#L1)
- Netlify deploy config: [netlify.toml](netlify.toml#L1-L200)

---

## Tech stack

- Static site generator: Hugo (site configured in `hugo.yaml`)
- Theme: Hextra (imported as a Hugo module; see `go.mod`)
- Build / deploy: Netlify (repo includes `netlify.toml`)
- Content format: Markdown

---

## Project structure

A quick overview of the repository layout and where to find things:

- Config: [hugo.yaml](hugo.yaml#L1-L200) — Hugo site configuration and menu/params.
- Module: [go.mod](go.mod#L1-L200) — Hugo module dependency (`hextra` theme).
- Content: [content/](content/_index.md#L1) — Markdown pages for the site (sectioned into `docs`, `ec-campus`, `rr-campus`, etc.).
- Static assets: `static/` — Images, CSS, and other files served as-is.
- Images: `pics/` — Additional image assets used across content.
- Deployment: [netlify.toml](netlify.toml#L1-L200) — Netlify build/deploy settings.
- Workflows: [workflows/hugo.yaml](workflows/hugo.yaml#L1-L200) — CI or workflow-related configs.
- Other folders: `auth/`, `samarpana/` — project-specific directories (site sections or asset groups).
- Root files: [README.md](README.md#L1-L200), [LICENSE](LICENSE#L1-L200)

---

## Prerequisites

Install the required tools on your machine:

- Install Hugo from https://gohugo.io/installation/. You can follow the instructions on the docs as per your OS.
- Git

## Development (local)

To run the site locally with drafts enabled:

```bash
hugo server --buildDrafts --disableFastRender
```

The server will start at `http://localhost:1313` by default.

---

## Contributing

We welcome contributions. A typical workflow:

1. Fork the repository.
2. Create a feature branch (e.g., `feature/update-docs`).
3. Make changes and commit.
4. Open a Pull Request describing your changes.
5. Optionally mention maintainers for review: [Siri N Shetty](https://github.com/siri-n-shetty) or [Achyuth S S](https://github.com/achyu-dev).

---

## License

This project is licensed under the MIT License.