# Technical Architecture

Demand2Market follows a serverless, edge-native architecture.

## Architecture Layers

### Presentation Layer

Built using:

- React
- TypeScript
- Vite
- Tailwind CSS

This layer provides separate experiences for customers and vendors.

---

### Application Layer

React services communicate with Supabase using authenticated sessions.

React Router manages application navigation.

---

### Data Layer

Supabase provides:

- PostgreSQL
- Authentication
- Realtime
- Row Level Security

Important data includes:

- Profiles
- Markets
- Products
- Vendor Products
- Demand Records
- Quality Feedback
- Purchase Verifications
- Rewards
- AI Quality Analysis

---

### Edge Layer

Supabase Edge Functions execute secure backend logic.

The `analyze-quality` Edge Function:

1. Authenticates the vendor.
2. Validates market access.
3. Reads relevant quality feedback.
4. Sends the analysis request to the AI provider.
5. Stores the resulting analysis.
6. Returns the result to the application.

---

### AI Layer

OpenRouter provides access to supported AI models.

The architecture also supports fallback models to reduce dependency on a single model.

---

### Deployment Layer

Frontend:

Vercel

Backend:

Supabase Cloud

Source Control:

GitHub
