# Traveloop

Traveloop is a premium consumer travel planning prototype built with Next.js, React, Tailwind CSS, shadcn-style UI primitives, lucide-react, Framer Motion, Recharts, Zod, JWT auth helpers, and PostgreSQL-ready API routes.

## Run locally

```bash
npm install
npm run dev
```

Open `http://localhost:3000`.

## Database

The API routes are PostgreSQL-ready and use `DATABASE_URL` when provided. The UI ships with rich demo data so the product can be explored immediately.

Create the relational schema with:

```bash
psql "$DATABASE_URL" -f db/schema.sql
```
