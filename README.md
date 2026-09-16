# Busline Abuja

A responsive pre-launch website and working waitlist for Busline, an Abuja transport-booking concept focused on predictable arrival times, digital booking, and live bus tracking.

## Features

- Official Busline branding
- Responsive landing page
- Pre-launch waitlist form
- Persistent waitlist storage with Cloudflare D1
- Simulated booking and live-tracking product preview
- Duplicate-email protection

## Technology

- React 19
- Next.js 16
- Vinext and Vite
- TypeScript
- Cloudflare Workers and D1
- Drizzle ORM

## Run locally

Requirements:

- Node.js 22.13 or newer
- pnpm

```bash
pnpm install
pnpm run build
```

For local development:

```bash
pnpm run dev
```

## Database

The waitlist API expects a Cloudflare D1 binding named `DB`. The database schema is defined in `db/schema.ts`, and the generated migration is in `drizzle/`.

Apply the migration to your D1 database before using the waitlist form in production.

## Important folders

- `app/` — website pages, styles, and waitlist API
- `db/` — Drizzle database access and schema
- `drizzle/` — SQL migrations
- `public/` — Busline logo and public assets

## Privacy

Waitlist entries contain contact details. Keep the database private, restrict access, and follow applicable privacy and data-protection requirements.

## Status

Busline is currently in pre-launch. The booking and live-tracking interface is a product demonstration.
