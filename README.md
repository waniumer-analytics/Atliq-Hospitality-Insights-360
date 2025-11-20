                                         Atliq-Hospitality-Insights-360
Revenue contributors & booking distribution
![Revenue Contributors](/mnt/data/Screenshot 2025-11-20 104703.png)
Weekly trends (Revenue, Bookings, Occupancy)
![Weekly Trends](/mnt/data/Screenshot 2025-11-20 104717.png)
City / Room Class / Category analytics
![City & Room Analytics](/mnt/data/Screenshot 2025-11-20 104756.png)

Project Overview
This project analyzes the business performance of AtliQ Hospitality, a chain of luxury and business hotels across multiple Indian cities.
Using Power BI, the dashboard provides a 360° view of revenue trends, occupancy performance, booking behavior, cancellation rates, customer ratings, property comparison, and city-wise profitability.
The main objective is to help the hospitality team make data-driven decisions related to pricing, demand forecasting, property performance, customer experience, and strategic business expansion.

 Key Business Questions
•	How are revenue, occupancy, and bookings performing overall?
•	Which cities, room types, and platforms contribute the most to revenue?
•	How do weekdays and weekends impact business performance?
•	Which properties are underperforming and require attention?
•	How do cancellation rates and customer ratings affect revenue?
•	What are the weekly demand patterns and seasonality trends?
Key Insights
•	Total Revenue: 1.71B, but Occupancy is only 58% → large revenue opportunity
•	Cancellation Rate is high (25%), causing booking instability
•	Mumbai contributes ~40% of total revenue, making it the strongest market
•	AtliQ Exotica, Palace & City contribute over 50% of all revenue
•	AtliQ Seasons underperforms with low revenue and poor rating (2.29)
•	Weekdays generate more revenue, while weekends push occupancy
•	Elite & Standard rooms dominate bookings, while Premium & Presidential drive higher revenue per booking
•	Week 32 shows an abnormal drop in revenue & bookings → requires investigation

What’s Included in the Dashboard
•	Overview / Executive KPIs: Revenue, RevPAR, ADR, DSRN, Occupancy %, Realisation %, Cancellation %, Avg Rating.
•	Weekday vs Weekend split: Separate KPI tiles for each to reveal different demand profiles.
•	Revenue Contributors: Top properties, cities, platforms, room classes and categories.
•	Key Metrics by Property: Revenue, Occupancy, Cancellation, Capacity, Rating.
•	Booking % by Room Class: Treemap / distribution visualization.
•	Weekly Trends: Time series for Revenue, Bookings, Occupancy with weekly granularity.
•	Segment Analytics: City-level, Room-class, Category (Business vs Luxury) performance and revenue-per-booking.

                                                    Tools & Technologies Used
•	Power BI
o	DAX Measures
o	Data Modeling (Star Schema)
o	Relationships & Calculations
o	Interactive Visualizations & Slicers
•	Excel/CSV (Data Source)
•	Power Query for data cleaning
•	GitHub for version control & documentation

                                                                  KPIs Tracked
Net Revenue
NetRevenue = SUM(Bookings[Revenue]) - SUM(Bookings[Commission])
Occupancy %
OccupancyPct = DIVIDE(SUM(Bookings[OccupiedRoomNights]), SUM(Calendar[SellableRoomNights]))
ADR (Average Daily Rate)
ADR = DIVIDE([NetRevenue], SUM(Bookings[OccupiedRoomNights]))
RevPAR
RevPAR = [ADR] * [OccupancyPct]
Cancellation Rate
Cancellation Rate = DIVIDE(SUM(Bookings[CancelledBookings]), SUM(Bookings[TotalBookings]))
Keep DAX measures centralized in a Measures table and document their definitions in docs/KPI_Definitions.md.


Business Impact
•	Improved visibility into city-wise and property-wise profitability
•	Clear identification of high-risk areas (cancellations, low occupancy)
•	Better revenue strategy using room class trends
•	Data-driven roadmap for operational improvements
Future Enhancements
•	Forecasting model for demand prediction
•	Integration of sentiment analysis from guest reviews
•	Real-time occupancy & revenue monitoring
•	Automated alerts for sudden revenue drops

 Recommendations (Short List)
1.	Strengthen Direct Booking channel and loyalty incentives.
2.	Introduce conditional non-refundable pricing to reduce cancellations.
3.	Implement targeted weekday offers (corporate packages) to raise occupancy.
4.	Prioritize service improvements for low-rating properties.
5.	Add a data quality & anomaly detection check (e.g., flag sudden weekly drops).

How to Use 
1.	Place your cleaned stock data (bookings, properties, calendar) into data/ folder.
2.	Open powerbi/AtliQ_Hospitality.pbix in Power BI Desktop.
3.	Use Power Query to connect to the CSV/Excel files and refresh.
4.	Verify relationships: Calendar ← Bookings ← Properties ← Platforms (star schema).
5.	Refresh visuals; validate totals against source data.

 Contact 
•	Owner: WANI UMAR 
•	Email :-
•	LINKEDIN:-
•	GITHUB:- 

