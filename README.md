# Traveloop – Modern Travel Planning Platform

Traveloop is a premium travel planning application designed for modern travelers. Plan trips, organize itineraries, manage budgets, and share trips with friends—all with a beautiful, intuitive interface.

## Features

- **Trip Planning**: Create and manage multiple trips with destinations, dates, and travelers
- **Itinerary Builder**: Organize activities by day with timeline visualization
- **Budget Tracking**: Track costs across categories (transport, stay, food, activities)
- **City Discovery**: Explore destinations with curated information
- **Packing Checklist**: Stay organized with reusable packing lists
- **Trip Sharing**: Generate shareable links for collaborative planning
- **Profile Management**: Personalize your travel experience

## Tech Stack

### Frontend
- Next.js 15+ with App Router
- React 18+
- Tailwind CSS
- shadcn/ui components
- Lucide React icons
- Recharts for visualizations
- Framer Motion for animations

### Backend
- Next.js API Routes
- Node.js runtime

### Database
- PostgreSQL
- Prisma ORM

### Authentication
- JWT-based authentication
- Password hashing with bcryptjs

## Getting Started

### Prerequisites
- Node.js 18+
- PostgreSQL 14+
- npm or yarn

### Installation

```bash
# Clone repository
git clone https://github.com/NoOne-444/odoo-X-Travelloop.git
cd odoo-X-Travelloop

# Install dependencies
npm install

# Setup environment variables
cp .env.example .env.local

# Setup database
npx prisma migrate dev

# Seed demo data (optional)
npm run seed

# Run development server
npm run dev
```

Visit `http://localhost:3000`

## Project Structure

```
traveloop/
├── app/
│   ├── api/                 # API routes
│   │   ├── auth/           # Authentication endpoints
│   │   ├── trips/          # Trip management
│   │   ├── cities/         # City search & discovery
│   │   ├── activities/     # Activity search
│   │   └── ...
│   ├── (auth)/             # Auth pages (login, signup)
│   ├── (dashboard)/        # Protected dashboard pages
│   ├── layout.tsx          # Root layout
│   └── page.tsx            # Landing page
├── components/
│   ├── ui/                 # reusable UI components
│   ├── cards/              # Card components
│   ├── forms/              # Form components
│   ├── navigation/         # Nav components
│   └── ...
├── lib/
│   ├── auth.ts            # Auth utilities
│   ├── db.ts              # DB connection
│   ├── api-client.ts      # API client
│   └── utils.ts           # General utilities
├── prisma/
│   ├── schema.prisma      # Database schema
│   └── seed.ts            # Seed data
├── public/                # Static assets
└── styles/                # Global styles
```

## API Documentation

See `/docs/API.md` for detailed API endpoints.

## Deployment

### Vercel (Recommended)
```bash
npm install -g vercel
vercel
```

### Docker
```bash
docker build -t traveloop .
docker run -p 3000:3000 traveloop
```

## License

MIT

## Support

For questions or issues, please open an issue on GitHub.
