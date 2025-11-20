                                         Atliq-Hospitality-Insights-360
Executive Summary
<img width="1397" height="648" alt="Executive Summary" src="https://github.com/user-attachments/assets/3b4071cc-fcf3-46e1-a67a-1f8afd9612ea" />
Property Performance
<img width="1277" height="836" alt="Property Performance" src="https://github.com/user-attachments/assets/1e2a6722-951b-4e1f-bcb7-e7924d7b84cc" />

Weekly trends (Revenue, Bookings, Occupancy)
<img width="1153" height="642" alt="Weekly Trends" src="https://github.com/user-attachments/assets/7a9d7ab5-e6d6-4217-8767-4a827ff41397" />

City / Room Class / Category analytics
<img width="809" height="813" alt="City ,Class,category" src="https://github.com/user-attachments/assets/311df027-84f7-40ea-b968-38c6c77e2fab" />


                                                   Project Overview
This project analyzes the business performance of AtliQ Hospitality, a chain of luxury and business hotels across multiple Indian cities.
Using Power BI, the dashboard provides a 360° view of revenue trends, occupancy performance, booking behavior, cancellation rates, customer ratings, property comparison, and city-wise profitability. The main objective is to help the hospitality team make data-driven decisions related to pricing, demand forecasting, property performance, customer experience, and strategic business expansion.

                                                    Key Business Questions
•	How are revenue, occupancy, and bookings performing overall?
•	Which cities, room types, and platforms contribute the most to revenue?
•	How do weekdays and weekends impact business performance?
•	Which properties are underperforming and require attention?
•	How do cancellation rates and customer ratings affect revenue?
•	What are the weekly demand patterns and seasonality trends?


                                                       Key Insights
                                                       
•	Total Revenue:-  1.71B, but Occupancy is only 58% → large revenue opportunity.
•	Cancellation Rate is high (25%), causing booking instability.
•	Mumbai contributes ~40% of total revenue, making it the strongest market.
•	AtliQ Exotica, Palace & City contribute over 50% of all revenue.
•	AtliQ Seasons underperforms with low revenue and poor rating (2.29).
•	Weekdays generate more revenue, while weekends push occupancy.
•	Elite & Standard rooms dominate bookings, while Premium & Presidential drive higher revenue per booking.
•	Week 32 shows an abnormal drop in revenue & bookings → requires investigation.


                                           What’s Included in the Dashboard
                                           
•	Overview / Executive KPIs:-   Revenue, RevPAR, ADR, DSRN, Occupancy %, Realisation %, Cancellation %, Avg Rating.
•	Weekday vs Weekend split:-   Separate KPI tiles for each to reveal different demand profiles.
•	Revenue Contributors:-   Top properties, cities, platforms, room classes and categories.
•	Key Metrics by Property:-   Revenue, Occupancy, Cancellation, Capacity, Rating.
•	Booking % by Room Class:-  Treemap / distribution visualization.
•	Weekly Trends:-   Time series for Revenue, Bookings, Occupancy with weekly granularity.
•	Segment Analytics:-   City-level, Room-class, Category (Business vs Luxury) performance and revenue-per-booking.

                                                    Tools & Technologies Used
                                                    
•	Power BI.
o	DAX Measures.
o	Data Modeling (Star Schema).
o	Relationships & Calculations.
o	Interactive Visualizations & Slicers.
•	Excel/CSV (Data Source).
•	Power Query for data cleaning.
•	GitHub for version control & documentation.

                                                                 
                                                                  KPIs Tracked

NetRevenue = SUM(Bookings[Revenue]) 

OccupancyPct = DIVIDE(SUM(Bookings[OccupiedRoomNights]), SUM(Calendar[SellableRoomNights])).
ADR (Average Daily Rate) = DIVIDE([NetRevenue], SUM(Bookings[OccupiedRoomNights])).
RevPAR = [ADR] * [OccupancyPct].
Cancellation Rate = DIVIDE(SUM(Bookings[CancelledBookings]), SUM(Bookings[TotalBookings])).
Keep DAX measures centralized in a Measures table and document their definitions in docs/KPI_Definitions.md.


                                           Business Impact
                                           
•	Improved visibility into city-wise and property-wise profitability.
•	Clear identification of high-risk areas (cancellations, low occupancy).
•	Better revenue strategy using room class trends.
•	Data-driven roadmap for operational improvements.

                                           
                                       Recommendations 
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
•	Email :-umar.1analytics@gmail.com 
•	LINKEDIN:- www.linkedin.com/in/waniumer-analytics 
•	GITHUB:- 

