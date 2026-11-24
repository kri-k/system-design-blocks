# System Design Blocks

A searchable, interview-focused catalog of system architecture building blocks, including when to use them, pros, cons, implementations and senior-level interview questions.

## Run locally

Requires Node.js 20+.

```bash
npm install
npm run dev
```

## Production build

```bash
npm run build
npm run preview
```

## Publish on GitHub Pages

1. Create a GitHub repository (for example `system-design-blocks`).
2. Commit and push this project to the `main` branch.
3. In GitHub **Settings → Pages**, select **GitHub Actions** as the build/deployment source.
4. The workflow in `.github/workflows/deploy.yml` builds and deploys the site automatically on pushes to `main`.

`vite.config.ts` uses `base: './'` so assets work under a repository subpath.

## Add or edit blocks

All catalog content is in `src/data.ts`. Each entry contains category, name, kind, description, when to use, pros, cons, implementations, and interview questions. Semicolons separate multiple entries in the compact data source.

## Future plans

- Architecture canvas with React Flow
- Compare components
- More detailed failure modes and design patterns
- Export diagrams

This is a study resource, not a substitute for workload-specific benchmarking and architecture review.
