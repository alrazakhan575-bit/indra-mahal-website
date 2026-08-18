# Indra Mahal Backend

Express + MongoDB API for the Indra Mahal hotel website.

## Local setup

```bash
cd backend
npm install
cp .env.example .env
npm run dev
```

Set `MONGODB_URI` in `.env` for persistent bookings and enquiries.

## Endpoints

- `GET /api/health` — health check
- `POST /api/enquiries` — create contact/event/dining enquiry
- `POST /api/bookings` — create room booking
- `GET /api/bookings` — list recent bookings (admin protection should be added before production)

## Production

Deploy the `backend` directory to a Node-compatible host such as Render or Railway. Keep secrets in the host's environment-variable settings; never commit `.env`.
