# myscraps

Personal mini tech notes, publicly.

---

## About

### Overview

A personal TIL-style tech blog built with Astro.js.
Insights gained during development are generalized and published as monthly notes.

### Purpose

This project has two aspects:

**Writing tech notes:**

- To use as a personal reference — look up past solutions quickly
- To improve learning by putting thoughts into words

**Publishing as a static site:**

- To _practice front-end development_ (Astro.js, etc.) in a real project
- To make notes accessible from anywhere, without login
- To improve searchability with tags, search, and better UI (planned)

---

## For Users

<!--
TODO: Decide whether this section is needed.
See: TODO.md (Backlog)
-->

---

## For Developers

### Policy

- **Use this project as a front-end learning playground.**
  Treat it as a place to practice Astro.js and front-end development in general.
- **Keep the code simple.**
  Avoid unnecessary complexity.
- **Keep maintenance cost low.**
  This project should be easy to return to after a long break.
- **Keep all documentation in the repository.**
  Do not use GitHub Wiki or Issues. All docs live in `.md` files in the repo.

### Tech Stack

| Category                | Tool         |
| ----------------------- | ------------ |
| Framework               | Astro.js     |
| Theme                   | AstroPaper   |
| Styling                 | Tailwind CSS |
| Language                | TypeScript   |
| Package manager         | npm          |
| Runtime version manager | mise         |
| Deployment              | Vercel       |
| Repository hosting      | GitHub       |
| CI                      | —            |

### Directory Structure

```
.
├── src/
│   ├── components/      # UI components (AstroPaper)
│   ├── layouts/         # Page layouts (AstroPaper)
│   ├── pages/           # Routes / pages (AstroPaper)
│   ├── styles/          # Global styles (AstroPaper)
│   ├── utils/           # Utility functions (AstroPaper)
│   ├── data/
│   │   └── blog/        # TIL posts (monthly .md files)
│   ├── config.ts        # Site-wide settings (title, author, URL, etc.)
│   └── constants.ts     # Social links and share links
├── public/              # Static assets
├── ADR.md               # Architecture Decision Records
├── TODO.md              # Task management
└── astro.config.ts      # Astro configuration
```

### Setup

**Prerequisites:**

- [Git](https://git-scm.com/)
- [mise](https://mise.jdx.dev/) — manage the Node.js version
- Node.js — installed via mise

```bash
# 1. Clone the repository
git clone https://github.com/rnazmo/myscraps.git
cd myscraps

# 2. Install Node.js via mise (version is pinned in .mise.toml)
mise install

# 3. Install dependencies listed in package.json
npm install

# 4. Start local dev server
npm run dev
# => Open http://localhost:4321 in your browser
```

### Conventions

TODO: To be defined.

### Workflows

#### Writing a new post

```bash
# Start local dev server and open http://localhost:4321
npm run dev
```

Edit or create a monthly file in `src/data/blog/`, then check the result in your browser.

#### Checking the production build locally

```bash
# Build and start a local preview server
npm run build
npm run preview
# Open http://localhost:4321 in your browser
```

#### Deploying to production

```bash
git push origin main
```

Pushing to `main` triggers an automatic deployment on Vercel.

### References

**This repository:**

- [TODO.md](./TODO.md)
- [ADR.md](./ADR.md)

**External:**

- [Astro.js docs](https://docs.astro.build/)
- [AstroPaper](https://github.com/satnaing/astro-paper)
