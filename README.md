# Hospitality-Insights

## Project Overview

AtliQ Grands owns multiple five-star hotels across India. They have been in the hospitality industry for the past 20 years. Due to strategic moves from other competitors and ineffective decision-making in management, AtliQ Grands are losing its market share and revenue in the luxury/business hotels category. As a strategic move, the managing director of AtliQ Grands wanted to incorporate “Business and Data Intelligence” to regain their market share and revenue.

## Objective

The objective of this project is to be able to exploit all the data provided by AtliQ Grands in order to analyze the different performances carried out and thus help AtliQ managers to make relevant decisions allowing them to move up and regain their leadership position.

I worked on this project by following the Codebasics PowerBi Course, Link to the course is [here](https://codebasics.io/courses/power-bi-data-analysis-with-end-to-end-project)

Take a look at the live Dashboard by clicking [here](https://app.powerbi.com/view?r=eyJrIjoiMjBkN2RiOWUtYzExNC00OWVmLTk3NTctN2QxMDZmM2RlZDkwIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

## Tech stacks

- Power BI Desktop
- Excel
- DAX language
- Project charter file

## PowerBI techniques used
-Data Loading, transforming and Loading
- Data modeling
- Creating calculated columns
- creating measure using DAX language
- creation of a button to clear all applied filters
- Using divide function to prevent zero division errors
- creating DAX Measures
- Data validation techniques
- Power BI services
- Publishing reports to Power BI services
- And more


## Business related terms

- Revenue
- Occupancy pourcentage
- Average rating
- ADR(Average Daily rate)
- RevPAR(Revenue Per Available Room)
- DBRN(Daily Booked Room Nights)
- DSRN(Daily Sellable Room Nights)
- DURN(Daily Utilized Room Nights)

### Different KPI visualized

- Revenue
- Average rating
- Occupancy rate
- successful bookings
- Cancellation rate
- Occupancy trend by day
- Bookings by room class
- Rate of bookings status
- Revenue by city
- Booking by platform
- Average rating by city
- Occupancy by city
- Occupancy by Day type


### Dataset **Understanding.**

Understanding what data is available will be more helpful while doing analysis. before jumping on to the analysis get good understanding of what are data available.

Dimension table : It will have the static data like details of hotels and rooms

Fact table : It will have the data about bookings  

Here are available data tables used for this analysis:
1. dim_date
2. dim_hotels
3. dim_rooms
4. fact_aggregated_bookings
5. fact_bookings

Column Description for dim_date:
1. date: This column represents the dates present in May, June and July.
2. mmm yy: This column represents the date in the format of mmm yy (monthname year).
3. week no: This column represents the unique week number for that particular date.
4. day_type: This column represents whether the given day is Weekend or Weekeday.

Column Description for dim_hotels:
1. property_id: This column represents the Unique ID for each of the hotels.
2. property_name: This column represents the name of each hotel.
3. category: This column determines which class[Luxury, Business] a particular hotel/property belongs to. 
4. city: This column represents where the particular hotel/property resides in.

Column Description for dim_rooms:
1. room_id: This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.
2. room_class: This column represents to which class[Standard, Elite, Premium, Presidential] particular room type belongs.

Column Description for fact_aggregated_bookings:
1. property_id: This column represents the Unique ID for each of the hotels.
2. check_in_date: This column represents all the check_in_dates of the customers.
3. room_category: This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.
4. successful_bookings: This column represents all the successful room bookings that happen for a particular room type in that hotel on that particular date.
5. capacity: This column represents the maximum count of rooms available for a particular room type in that hotel on that particular date.

Column Description for fact_bookings:
1. booking_id: This column represents the Unique Booking ID for each customer when they booked their rooms.
2. property_id: This column represents the Unique ID for each of the hotels
3. booking_date: This column represents the date on which the customer booked their rooms.
4. check_in_date: This column represents the date on which the customer check-in(entered) at the hotel.
5. check_out_date: This column represents the date on which the customer check-out(left) of the hotel.
6. no_guests: This column represents the number of guests who stayed in a particular room in that hotel.
7. room_category: This column represents the type of room[RT1, RT2, RT3, RT4] in a hotel.
8. booking_platform: This column represents in which way the customer booked his room.
9. ratings_given: This column represents the ratings given by the customer for hotel services.
10. booking_status: This column represents whether the customer cancelled his booking[Cancelled], successfully stayed in the hotel[Checked Out] or booked his room but not stayed in the hotel[No show].
11. revenue_generated: This column represents the amount of money generated by the hotel from a particular customer.
12. revenue_realized: This column represents the final amount of money that goes to the hotel based on booking status. If the booking status is cancelled, then 40% of the revenue generated is deducted and the remaining is refunded to the customer. If the booking status is Checked Out/No show, then full revenue generated will goes to hotels.


## Data Model

- Data modeling plays a vital role and is considered as the basement of report. All the visuals will be build upon the data model.
- Poor data modeling affects the over all performance of the report.
- Click [here](https://github.com/samarita22/Hospitality-Insights/blob/main/Data%20modeling.PNG) to visualize the data modeling


## Project Outcome

By using this report, decisions can be taken based on the data. Further it will help AtliQ Grands managers making relevant decisions allowing them to move up and regain their leadership position.
