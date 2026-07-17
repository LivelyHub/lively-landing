<p align="center">
  <img src="lively-landing/public/logo.png" alt="Lively logo" width="96" />
</p>

<h1 align="center">lively-landing</h1>

<p align="center">Marketing site for <strong>Lively</strong> — a WhatsApp companion that coaches Indonesian elders through daily strength exercise, while keeping family in the loop.</p>

> [!NOTE]
> Built for **Garuda Hacks 7.0** (Health track). Part of a four-repo system — `lively-landing`, `lively-mobile`, `lively-backend`, `lively-bot` — sharing a common data/API contract documented in [CORE.md](CORE.md). This site is static and doesn't call the Lively API at MVP.

## About

Lively pairs an elderly parent with a WhatsApp companion persona (Mbak Asih or Mas Budi) who checks in daily, runs a 30-second Chair Stand fall-risk assessment, and encourages short strength exercises — while the family monitors progress and safety alerts from a companion mobile app. This repo is the public-facing pitch: positioning, the problem (Indonesia's ageing population), how it works for both the elder and the family, and a call to action.

## Tech stack

- TypeScript, React 19, Vite 8 (with the React Compiler babel plugin)
- Tailwind CSS + shadcn/ui + reactbits for styling and components
- ESLint (typescript-eslint) for linting

## Getting started

> [!NOTE]
> The app lives one directory down, in [`lively-landing/`](lively-landing).

### Prerequisites

- Node.js 20+

### Install and run

```bash
cd lively-landing
npm install
npm run dev       # starts the Vite dev server
```

| Command | Description |
|---|---|
| `npm run dev` | Start the dev server |
| `npm run build` | Type-check and build for production |
| `npm run preview` | Preview a production build locally |
| `npm run lint` | Run ESLint |

### Configuration

No environment variables are required — this is a static site with no API calls or secrets. `.env.example` is kept mostly empty for consistency with the other Lively repos.

## Project structure

```
lively-landing/
├── public/          # logo, favicon, static assets
└── src/
    ├── App.tsx       # main pitch page (hero, problem, how-it-works, CTA)
    ├── PrivacyPage.tsx
    └── assets/
```

