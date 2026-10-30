# Smart India Hackathon Workshop
## Date:30/10/2026
## Reference Number:26009975
## Name: L.Maria Shilpa

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution
AgriDirect AI is an end-to-end B2B/B2C digital agricultural marketplace and logistics platform designed to eliminate supply chain intermediaries by directly connecting farmers and Farmer Producer Organizations (FPOs) with consumers, institutional bulk buyers, and processors.

Core Architecture & Operational Mechanics
Direct Multi-Channel Marketplace: Connects growers and buyers directly through web, mobile applications, regional IVR voice calling, and WhatsApp conversational AI.

AI Demand & Price Forecasting: Analyzes historical market trends, weather patterns, and regional demand to recommend optimal harvesting schedules and target direct pricing.

Smart Route & Logistics Optimization: Utilizes Capacitated Vehicle Routing algorithms (CVRP) to consolidate farm-gate pickups across neighboring farm clusters and dispatch local 3PL partners efficiently.

Automated Direct Payouts & Escrow: Grants optional micro-advance working capital prior to harvest and releases final balance settlements instantly via UPI/bank transfer upon digital quality verification at pickup.

How It Addresses the Problem
Bypasses Intermediary Chains: Eliminates commissions from middlemen and commission agents, sharing the savings between higher farmer realization and lower consumer prices.

Eliminates Distress Sales: AI forecasting provides farmers market transparency before harvesting, preventing oversupply gluts and forced price cuts.

Optimizes Logistics Overhead: Dynamic vehicle route planning aggregates partial loads, drastically reducing transit delays and freight expenses.

Innovation and Uniqueness
Voice-First Rural Accessibility: Enables non-tech-savvy farmers to list crops, review prices, and accept advance funding via hands-free IVR calls or regional voice notes.

Dynamic Spatial Matchmaking: Uses graph-based location algorithms to connect bulk buyers with nearby farm clusters, reducing perishability and cold-chain transit to under 24 hours.

Transparent Digital QA Ledger: Employs mobile quality checklists and IoT-linked weighing scales at farm gates to prevent arbitrary quality deductions by traditional traders.

## Technical Approach

<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/676b3592-488c-4c44-a0d7-b8efcc8146e6" />


* **Frontend:** React Native/Flutter mobile apps for farmers/buyers; React.js admin web dashboard.
* **Backend:** Python FastAPI and Node.js managing RESTful microservices and API gateways.
* **AI & Optimization Engine:** PyTorch and LightGBM for demand forecasting; Google OR-Tools for route optimization (CVRP).
* **Database & Caching:** PostgreSQL with PostGIS for spatial queries; Redis for fast session caching.
* **Telephony & Messaging:** Twilio, Exotel, and WhatsApp Business APIs for regional IVR voice calls and automated messaging.
* **Cloud & Payment Escrow:** AWS/GCP hosting; Razorpay and UPI/DBT APIs for automated escrow hold and instant payouts.
* **Data Pipeline:** Continuous ingestion of *Agmarknet* price data, weather feeds, and crop calendars.
* **Logistics & QA Integration:** Automated 3PL routing linked to mobile quality-check sign-offs to trigger instant payments at pickup.

## Feasibility and Viability
Analysis of Feasibility
Technical Feasibility: Highly feasible due to mature, open-source vehicle routing engines (Google OR-Tools), scalable cloud microservices, and reliable regional telephony/WhatsApp APIs.

Financial Viability: Sustainable through a minimal 2%–3% platform fee charged to bulk buyers, remaining far lower than the traditional 15%–30% middleman commission margins.

Operational Feasibility: Leverages existing high rural smartphone penetration, widespread digital payment (UPI) networks, and local third-party logistics (3PL) infrastructure without requiring a capital-intensive fleet investment.

## Impact and Benefits

* **Target Audience Impact:** Empowers smallholder farmers, FPOs, and rural communities by providing direct market access, financial autonomy, and fair price discovery.

### Benefits Breakdown

* **For Farmers:**
* Increases net earnings by **20%–35%** by eliminating commission agent fees.
* Provides working capital advances to prevent distress selling.

* **For Consumers & Bulk Buyers:**
* Reduces final purchasing costs by **15%–20%** through supply chain consolidation.
* Ensures fresh, farm-direct produce with transparent quality standards.

* **For Logistics Partners:**
* Maximizes truck capacity utilization and minimizes empty return journeys using optimized routing.

### Broader Benefits

* **Social:** Financial inclusion via direct digital payments (UPI/DBT) and equal market visibility for small-scale growers.
* **Environmental & Waste Reduction:** Cuts post-harvest food waste by up to **25%** through fast, AI-optimized transit routes, reducing overall carbon emissions.

## Research and References
Ministry of Agriculture & Farmers Welfare (Agmarknet Portal): Data structures for agricultural commodity pricing, arrival volumes, and mandi trends across India.

NITI Aayog Agricultural Strategy Reports: Policy insights on post-harvest supply chain bottlenecks, FPO aggregation models, and direct farm-to-market channels.

Google OR-Tools Optimization Suite: Documentation and algorithms for solving Vehicle Routing Problems (VRP) with capacity and time constraints.

Smart India Hackathon (SIH) Open Dataset Guidelines: Architecture standards for agricultural technology solutions and direct digital marketplaces.
