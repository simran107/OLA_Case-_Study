

OLA BI Dashboard Overview
The Power BI dashboard contains multiple interactive visuals segregated into 5 key views:

Overall

Ride Volume Over Time

Booking Status Breakdown

Vehicle Type

Top 5 Vehicle Types by Ride Distance

Revenue

Revenue by Payment Method

Top 5 Customers by Total Booking Value

Ride Distance Distribution Per Day

Cancellations

Cancellation Reasons (Customer & Driver)

Ratings

Driver Ratings Distribution

Customer vs. Driver Ratings

Dataset Summary
The dataset simulates 1 lakh rows of OLA booking records for Bangalore city over one month. It includes:

Customer and Booking IDs

Vehicle Types: Auto, Bike, eBike, Prime Sedan, Prime SUV, etc.

Pickup/Drop Locations: 50 dummy Bangalore areas

Booking Status: Success, Cancelled, Incomplete

Ratings: Customer & Driver

TATs: VTAT & CTAT

Payment Methods & Booking Value

Data Constraints
Success rate: ~62%

Customer cancellations: ≤7%

Driver cancellations: ≤18%

Incomplete rides: ≤6%

Higher order volume & value on weekends and match days

 SQL Questions Covered

Retrieve all successful bookings

Average ride distance per vehicle type

Total cancelled rides by customers

Top 5 customers by total bookings

Rides cancelled by drivers for personal/car issues

Min/Max driver ratings for Prime Sedan

Rides with UPI payments

Avg. customer rating per vehicle type

Total booking value for successful rides

All incomplete rides and reasons


-- Average Ride Distance per Vehicle Type
SELECT Vehicle_Type, AVG(Ride_Distance) as avg_distance
FROM bookings
GROUP BY Vehicle_Type;
All queries have been saved as SQL Views for optimized analysis.

 Key Insights
 
Most Popular Vehicle Type: Prime Sedan by distance

Booking Peak Days: Weekends & Match Days

Top Payment Method: UPI & Cash

Customer Rating Trends: Higher ratings on successful rides

Cancellation Trends: Driver issues are more frequent than customer cancellations


