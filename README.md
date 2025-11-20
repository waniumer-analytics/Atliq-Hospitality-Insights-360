                                         Atliq-Hospitality-Insights-360
                                         
                                         DOMAIN:-  Hospitality Analytics 
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
                                                    
1. How are revenue, occupancy, and bookings performing overall?
2. 	Which cities, room types, and platforms contribute the most to revenue?
3. 	How do weekdays and weekends impact business performance?
4. 	Which properties are underperforming and require attention?
5. 	How do cancellation rates and customer ratings affect revenue?
6. 	What are the weekly demand patterns and seasonality trends?


                                                       Key Insights
                                                       
1. Total Revenue:-  1.71B, but Occupancy is only 58% → large revenue opportunity.
2. Cancellation Rate is high (25%), causing booking instability.
3. 	Mumbai contributes ~40% of total revenue, making it the strongest market.
4. 	AtliQ Exotica, Palace & City contribute over 50% of all revenue.
5. 	AtliQ Seasons underperforms with low revenue and poor rating (2.29).
6. Weekdays generate more revenue, while weekends push occupancy.
7. 	Elite & Standard rooms dominate bookings, while Premium & Presidential drive higher revenue per booking.
8. 	Week 32 shows an abnormal drop in revenue & bookings → requires investigation.


                                           What’s Included in the Dashboard
                                           
1. 	Overview / Executive KPIs:-   Revenue, RevPAR, ADR, DSRN, Occupancy %, Realisation %, Cancellation %, Avg Rating.
2. 	Weekday vs Weekend split:-   Separate KPI tiles for each to reveal different demand profiles.
3.  Revenue Contributors:-   Top properties, cities, platforms, room classes and categories.
4. 	Key Metrics by Property:-   Revenue, Occupancy, Cancellation, Capacity, Rating.
5. 	Booking % by Room Class:-  Treemap / distribution visualization.
6. 	Weekly Trends:-   Time series for Revenue, Bookings, Occupancy with weekly granularity.
7. 	Segment Analytics:-   City-level, Room-class, Category (Business vs Luxury) performance and revenue-per-booking.

                                                    Tools & Technologies Used
                                                    
1. 	Power BI.
2. 	DAX Measures.
3. 	Data Modeling (Star Schema).
4. 	Relationships & Calculations.
5. Interactive Visualizations & Slicers.
6. 	Excel/CSV (Data Source).
7. Power Query for data cleaning.
8. 	GitHub for version control & documentation.

                                                                 
                                                                  KPIs Tracked

1. NetRevenue = SUM(Bookings[Revenue]) 
2. OccupancyPct = DIVIDE(SUM(Bookings[OccupiedRoomNights]), SUM(Calendar[SellableRoomNights])).
3. ADR (Average Daily Rate) = DIVIDE([NetRevenue], SUM(Bookings[OccupiedRoomNights])).
4. RevPAR = [ADR] * [OccupancyPct].
5. Cancellation Rate = DIVIDE(SUM(Bookings[CancelledBookings]), SUM(Bookings[TotalBookings])).
6. Keep DAX measures centralized in a Measures table and document their definitions in docs/KPI_Definitions.md.


                                           Business Impact
                                           
1. 	Improved visibility into city-wise and property-wise profitability.
2. 	Clear identification of high-risk areas (cancellations, low occupancy).
3. 	Better revenue strategy using room class trends.
4.  Data-driven roadmap for operational improvements.

                                           
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
1.  Owner: WANI UMAR 
2. Email :-umar.1analytics@gmail.com 
3. 	LINKEDIN:- www.linkedin.com/in/waniumer-analytics 
4.  GITHUB:- https://github.com/waniumer-analytics/Atliq-Hospitality-Insights-360 

