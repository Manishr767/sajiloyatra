# SajiloYatra — Nepal Travel Frontend

SajiloYatra is a travel-planning web application concept focused on helping people explore destinations and travel experiences in Nepal. This repository contains the **Next.js frontend**.

> This is an evolving portfolio/learning project. Features and integrations may change as development continues.

## Frontend technology

- Next.js 15 (App Router)
- React 19
- JavaScript
- Prisma ORM
- SQLite for the local Prisma data model
- Axios for HTTP requests
- ESLint

## Current application areas

The source includes pages and components for:

- Home and destination discovery
- Trek listings and trek detail pages
- Lodging information
- Local experiences and events
- User login, registration, and profile screens
- Booking-related screens
- API route handlers for stories, treks, and lodging

The availability and completeness of individual workflows may vary.

## Run locally

### Requirements

- Node.js (use an LTS release compatible with Next.js 15)
- npm

### Setup

```bash
git clone https://github.com/Manishr767/sajiloyatra.git
cd sajiloyatra
npm install
```

The Prisma schema currently uses a local SQLite database at `prisma/dev.db`. If you are setting up a fresh environment, generate the Prisma client and apply the committed migrations:

```bash
npx prisma generate
npx prisma migrate deploy
```

Start the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## Useful scripts

| Command | Purpose |
|---|---|
| `npm run dev` | Start the development server |
| `npm run build` | Build for production |
| `npm run start` | Start the production server |
| `npm run lint` | Run ESLint |

## Database

The Prisma schema currently defines `Trek`, `Story`, and `Lodging` models. The checked-in schema uses SQLite for local development.

## Development notes

- Configure external API/base URLs through environment variables rather than hard-coding local addresses.
- Do not commit production credentials, API keys, or real user data.
- Add automated tests for important page and API behavior before treating the application as production-ready.

## Author

**Manish Rauniyar** · [GitHub](https://github.com/Manishr767)
