⚡ Power BI – Hotel Project with Power BI

---

📘 Project Overview

This is a multi-page Power BI dashboard built on a cleaned dataset of ~119K customer bookings (cleaned & preprocessed in Python).
The dashboard turns raw hospitality booking data into a decision-grade analytics product that answers business questions across bookings, customers, hotels, and revenue loss. It is built for executive overviews and analyst deep dives with clear navigation: Overview → Hotel → Customer → Revenue → Drill Through.

---

### ⚠️ Business Challenge

- Hotel operations and commercial teams lacked a single view to answer:

- Where are bookings and revenue coming from (by country, segment, hotel type)?

- Which customer segments drive the most cancellations or lost revenue?

- How to quantify lost revenue and prioritize actions to recover revenue and improve occupancy?

- Without a unified dashboard, stakeholders struggled to align pricing, distribution, and retention actions.

---

### 💡 Approach

- Data cleaning & ETL: cleaned 119K customer records in Python (deduplication, date parsing, missing value handling, standardizing categories).

- Data modeling: built a star-like model inside Power BI linking bookings, customers, hotel metadata, and revenue details.

- DAX & KPIs: created robust DAX measures for occupancy, cancellation rate, ADR, lost revenue, repeat-guest counts, and segment revenue.

- UX & navigation: designed a 4+ page experience with consistent KPI strip, filters (Hotel / Year), and drill-through for detail investigations.

- Visual design: custom theming and card-style KPI blocks for instant executive readability.

---

### 🖼️ Dashboard Pages & Key Visuals

- Overview (Overview screenshot) — Executive KPIs & trend lines:

- Total Booking, Total Revenue, Agents / Companies, Occupancy Rate, Cancellation Rate.

- Trend: bookings by year and top revenue countries.

- Hotel (Hotel page screenshot) — Hotel-level KPIs:

- City vs Resort bookings & occupancy, reservation status, booking by room type, occupancy by hotel.

- Customer (Customer page screenshot) — Customer behavior:

- Reserved vs canceled bookings, repeated guest counts, top booking countries, occupancy by customer type.

- Revenue (Revenue page screenshot) — Revenue & lost revenue analytics:

- Actual Revenue vs Lost Revenue over time, ADR (Average Daily Revenue), revenue by customer type & hotel.

- Drill Through — Detail-level investigation for single booking, customer, or hotel.

(Images used in README)

![Hotel](/Image/Hotel_Dashboard.png)
![Overview](/Image/Hotel_Overview.png)
![Customer](/Image/Customer_Overview.png)
![Revenue](/Image/revenue_Overview.png)

---

### 📊 Key Metrics (captured from the dashboard)
 Metric	Value (as shown)
- Total Bookings	119K
- Total Revenue	42.72M (aggregate displayed)
- Actual Revenue	26.00M
- Total Lost Revenue	16.73M
- Average Daily Revenue (ADR)	$101.83
- Total Occupancy Rate	62.96%
- Cancellation Rate	37.04%
- No. Reserved Booking	75K
- No. Cancelled Booking	44K
- No. Repeated Guests	3,810
- Top booking country (by volume)	PRT (~49K bookings)
- Top revenue by country	PRT (~14.1M)
- No. Booking City vs Resort	City: 79K — Resort: 40K
- Occupancy City / Resort	City: 58.27% — Resort: 72.24%

---

### 📈 Key Insights (what the dashboard revealed)

- High cancellation rate (37%) — cancellations represent a material part of lost revenue.

- Substantial lost revenue (16.73M) — a large share of potential revenue never realized due to cancellations, no-shows, and booking mismatches.

- Portugal (PRT) leads both bookings and revenue — strong market concentration that requires distribution & pricing focus.

- City hotels have more bookings but lower occupancy compared to resorts — opportunity to improve conversion/upsell in city properties.

- Online TA & OTAs dominate booking volume — distribution costs and cancellation profiles from these channels must be optimized.

- Repeat guests are low (3.8K) relative to base — retention tactics could significantly raise lifetime value.

---

### ⚠️ Problems Identified

- Overreliance on a few countries and distribution channels increases commercial risk.

- Cancellation patterns are creating a major revenue leakage.

- Low repeat-customer ratio indicates weak loyalty/retention mechanics.

- City properties show lower occupancy despite larger booking volume — pricing or channel mismatch likely.

---

### ✅ Recommendations

- Implement stricter cancellation policies or refundable deposit tiers for high-risk channels to reduce lost revenue.

- Target retention programs for guest segments with higher ADR (e.g., loyalty discounts, targeted follow-ups for repeat opportunities).

- Focus pricing & promotions by market (PRT and GBR are high-value markets) to optimize RevPAR.

- Channel optimization: negotiate with top OTAs to improve cancellation terms or promote non-refundable rates.

- A/B test deposit & refund rules for online TA bookings to measure impact on cancellations and occupancy.

- Build an early-warning lost revenue dashboard (alerts for sudden cancellation spikes by channel/hotel).

---

### 🧰 Tools & Techniques Used

- Python — data cleaning, deduplication, parsing dates, mapping categories (source of the 119K cleaned dataset).

- Power Query (Power BI) — ETL & lightweight transformations inside the data model.

- Power BI — modeling, DAX measures, page navigation, visuals, and report theming.

- DAX measures (examples):

1. TotalBookings = COUNTROWS(Bookings)

2. CancellationRate = DIVIDE([CancelledBookings], [TotalBookings])

3. OccupancyRate = DIVIDE([OccupiedRooms], [AvailableRooms])

4. ADR = DIVIDE([ActualRevenue], [TotalRoomNights])

5. LostRevenue = [PotentialRevenue] - [ActualRevenue]

Design — custom theming, KPI cards, and drill-through navigation for analyst workflows.

---
---

### 🔗 Interactive Dashboard
-📊 **Live Dashboard:** [**Click here**](https://app.powerbi.com/reportEmbed?reportId=b89059e0-536a-4e4d-aba2-b410510312a0&autoAuth=true&ctid=1158e2d5-dc24-41ad-abce-62841076dbde) --
-👉 [View on NovyPro](https://project.novypro.com/I9SBJA)

---

### 👤 Author
**Raafat Elrais**  
Business Intelligence Developer  

👤 Connect with me on LinkedIn: [Raafat Elrais](https://www.linkedin.com/in/raafat-elrais/)  

💡 #OpenToWork — always open to collaborations, BI projects, and opportunities in **Data Analytics, Visualization, and Business Intelligence.**

---

