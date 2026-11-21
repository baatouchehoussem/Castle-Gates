# Castle Gates

**Digital agency engineering automated WhatsApp booking platforms for hospitality & service SMEs.**

## Overview

Castle Gates builds end-to-end automated booking systems delivered through WhatsApp Business. Clients manage appointments, cancellations, reminders, and payments entirely within WhatsApp — no app download required for end users.

## Tech Stack

- **Backend**: Python, FastAPI
- **Messaging**: Twilio WhatsApp Business API
- **Database**: PostgreSQL
- **Deployment**: Docker Compose
- **Frontend**: Lightweight admin dashboard (HTML/JS)

## Features

- Conversational booking flow with natural language understanding
- Automated reminders & confirmations via WhatsApp templates
- Real-time availability sync with Google Calendar / Cal.com
- Multi-tenant architecture for agency white-label deployments
- Webhook-driven event processing (booking.created, booking.cancelled, payment.received)

## Quickstart

```bash
# Clone & configure
git clone https://github.com/baatouchehoussem/Castle-Gates
cd Castle-Gates
cp .env.example .env   # Add Twilio credentials, DB URL, webhook base URL

# Run with Docker Compose
docker compose up -d
```

## Project Structure

```
├── app/                 # FastAPI application
│   ├── api/             # REST endpoints + Twilio webhooks
│   ├── services/        # Booking logic, messaging, calendar sync
│   └── models/          # SQLAlchemy models
├── admin/               # Static admin dashboard
├── docker-compose.yml
└── .env.example
```

## License

Proprietary — contact for partnership inquiries.

---

*Built by [Houssem Baatouch](https://github.com/baatouchehoussem) — Founder, Castle Gates*