# nextjs

Next.js study repo with strict lint, TypeScript strict mode, UUIDv7 / CSPRNG rules, and minimal CI.

## Badges
![CI](https://github.com/unchain0/nextjs/workflows/CI/badge.svg)

## Real output

Terminal build result:

```
Route (app) Size First Load JS
○ / 5.68 kB 108 kB
```

Full log: `docs/assets/build-output.txt`

## Quick start

```bash
npm ci
npm run build
npm run lint
```

## Development rules

- Strict TypeScript (`noImplicitAny`, `strict`)
- ESLint with complexity limit (`max 10` cycles), `no-explicit-any`
- Warnings treated as errors; UUIDv7 / OS CSPRNG only
- Lockfile (`package-lock.json`) required; dependency audit in CI
