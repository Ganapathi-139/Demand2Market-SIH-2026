# Security

Security is an important part of Demand2Market's architecture.

## Row Level Security

PostgreSQL Row Level Security is used to restrict access to application data.

Examples:

- Customers access their own demand records.
- Vendors access data associated with their selected market.
- Rewards are scoped to customer and market.
- Quality information is restricted according to market permissions.

---

## API Keys

Public frontend configuration contains only the Supabase public client key.

Sensitive credentials are not exposed to the frontend.

Server-side secrets such as AI provider credentials are stored in the Supabase Edge Function environment.

---

## Authentication

The application uses Supabase authentication and authenticated sessions to associate application actions with users.

---

## Data Isolation

Market IDs and user IDs are used throughout the application to maintain data boundaries.

---

## Important Repository Rule

Never commit:

- `.env`
- Service-role keys
- AI API keys
- Database passwords
- Private credentials
- Customer personal data
