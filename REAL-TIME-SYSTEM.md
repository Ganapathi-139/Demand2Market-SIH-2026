# Real-Time System

Demand2Market uses Supabase Realtime to provide live application updates.

## Vendor

When a customer submits new demand:


   Customer
     ↓
  demand_records
     ↓
  Supabase Realtime
     ↓
 Vendor Dashboard
     ↓
Charts / Demand Data Updated

The vendor does not need to manually refresh the browser.

##Customer

When a reward is generated:

QR Verification
      ↓
purchase_verifications
      ↓
rewards
      ↓
Supabase Realtime
      ↓
Customer Dashboard

The customer's reward information can update immediately.

##Quality Feedback

Customer Feedback
       ↓
quality_feedback
       ↓
Realtime Event
       ↓
Vendor Quality Insights
