# Smart India Hackathon Workshop
# Date:30-10-2026
## Reference Number:26019319
## Name:Pugazh R

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

FarmLink Direct is a digital marketplace where farmers and FPOs can list produce for households, retailers, hotels, processors, and institutional buyers. It combines buyer discovery with shared logistics and clear transaction records.
- Farmers or FPOs create a listing with crop, quantity, harvest or dispatch date, location, expected price, and available quality details. Listings can be entered through a mobile app, assisted service centre, or FPO representative.
- Buyers can search and filter listings by commodity, quantity, location, quality, and delivery date. They can make an offer or place an order, with the full price and delivery terms shown before confirmation.
- A quality card records grading or test results where available. Buyers can request inspection or sampling before dispatch; the platform will distinguish verified information from seller-provided details.
- Orders can be grouped by village, collection point, commodity, or route. The platform matches them with available transport and storage services and displays the delivery charge separately.
- Farmers receive order updates and digital payment records. A transaction ledger shows quantity, agreed price, service charges, delivery status, and payment status to both parties.
- A demand dashboard helps FPOs plan aggregation and harvest scheduling. Forecasts are decision support only; farmers retain control over what they list and the price they accept.
- The platform supports local languages and low-bandwidth use, with SMS or messaging alerts for key steps such as offer received, order confirmed, pickup, delivery, and payment.
The distinctive focus is on transparent net returns: users can compare buyer offers after disclosed transport and service costs, instead of seeing a headline price alone.

## Technical Approach

Architecture and components
1. User channels: Responsive web and Android interfaces for farmers, FPOs, buyers, and logistics providers; assisted listing and SMS notifications for users with limited connectivity.
2. Marketplace services: APIs for registration, produce listings, buyer search, offers, order management, and dispute records. Role-based access protects personal, financial, and business information.
3. Data layer: A relational database for accounts, listings, orders, and payments; object storage for produce images and quality documents; an audit log for changes to prices, quantities, and order status.
4. Integrations: Where permitted, use public market-price and commodity information as reference data. Payment and identity checks should use authorized providers and require user consent. The platform should complement existing market systems and comply with applicable state market rules.
5. Demand forecasting: Begin with transparent baselines using historical orders, seasonality, local prices, weather or calendar signals where lawful and available, and buyer intent. Show forecast ranges and confidence, and evaluate accuracy against actual orders before expanding.
6. Logistics optimization: Match orders to vehicle capacity, pickup windows, delivery locations, and produce handling needs. Start with route clustering and distance-based estimates; incorporate traffic or live routing data only when reliable data access is available.
7. Security and reliability: Encrypt data in transit and at rest, use access controls and backups, minimize stored personal data, and maintain an incident and grievance process.
Implementation flow
Farmer/FPO lists produce
          ↓
Quality and quantity details recorded
          ↓
Buyers discover listings and make offers
          ↓
Farmer/FPO compares net proceeds and accepts
          ↓
Orders grouped and transport assigned
          ↓
Pickup → delivery confirmation → payment record
          ↓
Transaction data improves planning and forecasts
Pilot methodology
- Start in one produce cluster with a small set of FPOs, buyers, and transporters.
- Validate listing, price comparison, order confirmation, delivery, and payment records through real transactions.
- Track forecast error, fulfilment rate, delivery cost per unit, time to payment, repeat buyers, and farmer net realization.
- Improve the workflow from user feedback before adding commodities or locations.

- <img width="1600" height="1000" alt="WhatsApp Image 2026-10-30 at 9 23 26 PM" src="https://github.com/user-attachments/assets/a304ac72-4612-4f46-b8f5-85049c4d69fc" />



## Feasibility and Viability

The idea is feasible as a staged marketplace because its first version can rely on standard mobile and web technology, manual onboarding, and existing transport providers. It does not require the platform to own warehouses or vehicles.
Operational viability
- FPOs can aggregate produce and help with onboarding, listing accuracy, grading, and collection-point coordination.
- Existing transporters can be onboarded with vehicle type, capacity, route, and availability. Shared loads can improve vehicle utilization where order volume permits.
- Buyers can include local retailers and food businesses as well as bulk buyers, giving the pilot more than one demand channel.
- Payments should use authorized payment partners, with settlement terms shown clearly and reconciled against delivery records.
Key challenges and responses
- Unreliable supply or listing details: Confirm quantity and dispatch date before accepting orders; allow buyers to request inspection; record changes and cancellations.
- Quality disputes: Use simple commodity-specific grading fields, optional sampling, timestamped photos, and a documented dispute process.
- Thin demand and fragmented orders: Pilot in a concentrated geography and commodity cluster; prioritize repeat institutional buyers and aggregate nearby orders.
- Transport cost or delays: Show delivery charges before order acceptance, provide pickup windows, and track fulfilment and delay reasons.
- Digital access and trust: Offer assisted onboarding through FPOs, local-language interfaces, simple receipts, and support by phone or messaging.
- Regulatory variation: Check applicable state APMC and direct-trade requirements before operating in each location; obtain legal and payment-partner review for the pilot.
Viability measures
Assess the pilot using farmer net realization after disclosed costs, buyer price versus relevant local benchmarks, percentage of orders delivered in full and on time, average logistics cost per unit, time from delivery to payment, repeat purchase rate, and dispute rate. Expand only if the pilot shows consistent demand and acceptable fulfilment.

## Impact and Benefits

For farmers and FPOs
- More buyer options and clearer offers can improve bargaining power.
- Comparing offers after transport and service costs helps farmers judge actual net proceeds.
- Aggregated listings can make small lots visible to buyers that need larger quantities.
- Order and payment records support better planning, accountability, and repeat business.
For consumers and buyers
- Buyers can compare source, quantity, quality information, price, and delivery terms in one place.
- Better coordination may reduce avoidable handling and transport steps, which can contribute to more competitive prices.
- Small businesses and institutions can discover nearby suppliers and plan purchases against expected availability.
For the supply chain and environment
- Grouped pickups and route planning may improve vehicle utilization and reduce unnecessary trips.
- Better demand visibility can help align aggregation and dispatch with confirmed orders, potentially reducing unsold or delayed produce.
- Transaction data can identify recurring bottlenecks such as late pickup, quality rejection, or high delivery cost.
Measurement plan
Establish a baseline before the pilot and compare it with pilot transactions. Report farmer net realization, buyer price, logistics cost per kilogram, delivery completion and delay rates, time to payment, repeat orders, quality disputes, and produce left unsold. Environmental benefits should be reported only where vehicle or trip data supports a measured estimate.

## Research and References

These sources support the design choices around digital agricultural markets, quality information, FPO aggregation, logistics, and post-harvest management:
1. National Agriculture Market (e-NAM), Operational Guidelines — Describes market operations, assaying, electronic payment, logistics, and dispute handling. Useful for designing compatible transaction and quality workflows.
   e-NAM Operational Guidelines (PDF)
2. e-NAM, Assaying — Explains the role of produce testing and how assaying information can be used in trading.
   e-NAM Assaying
3. Small Farmers’ Agribusiness Consortium (SFAC), FPO Guidelines — Provides official guidance on formation and promotion of FPOs, relevant to farmer aggregation and onboarding.
   SFAC Guidelines
4. Indian Council of Agricultural Research, Vision 2030 — Discusses supply-chain inefficiencies and approaches including linking producers to markets, local value addition, and storage.
   ICAR Vision 2030 (PDF)
5. e-NAM, Trading Details — Describes platform features including logistics information, FPO participation, and warehouse-based trading.
   e-NAM Trading Details
