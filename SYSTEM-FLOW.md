# System Flow

## Overall Flow

                CUSTOMER
                   |
                   v
          Select Local Market
                   |
                   v
          Select Available Product
                   |
                   v
          Enter Expected Quantity
                   |
                   v
            Demand Record
                   |
                   v
          PostgreSQL / Supabase
                   |
                   v
          Market-Level Analysis
                   |
          +--------+--------+
          |                 |
          v                 v
    Demand Forecast     Quality Data
          |                 |
          v                 v
    Vendor Dashboard     AI Analysis
          |                 |
          +--------+--------+
                   |
                   v
          Vendor Decision Support
                   |
                   v
          Better Procurement


Real-Time Flow

     Customer Action
         |
         v
    Supabase Database
         |
         v
    Supabase Realtime
         |
         v
    Vendor / Customer Application
         |
         v
    UI Updates Automatically

QR Reward Flow

    Customer Purchase
        |
        v
      QR Scan
        |
        v
    Purchase Verification
        |
        v
    Duplicate Check
        |
        v
    Reward Token
        |
        v
    Monthly Streak Update
        |
        v
    Customer Reward Dashboard
