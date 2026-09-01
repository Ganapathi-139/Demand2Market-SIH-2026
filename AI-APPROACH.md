# AI Approach

Demand2Market uses Generative AI to transform raw customer feedback into understandable vendor insights.

## Quality Analysis

Customers submit:

- Product
- Rating
- Optional comment

The information is stored in PostgreSQL.

The secure Edge Function collects relevant feedback and sends it to the AI provider.

The AI produces:

- Overall quality score
- Freshness score
- Sentiment
- Positive points
- Common problems
- Recommendation

---

## AI Architecture

   Customer Feedback
       |
       v
   PostgreSQL
       |
       v
   Supabase Edge Function
       |
       v
   OpenRouter
       |
       v
    AI Model
       |
       v
  Structured Quality Analysis
       |
       v
   PostgreSQL
       |
       v
  Vendor Dashboard
