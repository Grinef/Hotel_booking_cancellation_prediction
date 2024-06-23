# Hotel Booking Cancellation Prediction Project

## Project Overview
The client, a hotel chain "Like a Guest," has added an option on their website to book rooms without prepayment to attract more customers. However, cancellations result in financial losses for the hotel. To mitigate this, the hotel wants a system that predicts booking cancellations. If a booking is likely to be canceled, the system will prompt the customer to pay a deposit, which is 80% of the room cost for one night plus one-time cleaning costs. This deposit will be charged if the customer cancels the booking.

## Business Metric and Additional Data
The primary business metric for the hotel chain is profit, which is the difference between the room's total cost and the service costs. The hotel has various room types, each with specific nightly rates and cleaning costs. Cleaning is done every two days for extended stays. Seasonal coefficients affect the pricing: spring and autumn have a 20% increase, while summer has a 40% increase.

### Room Costs:
- **Category A**: 1000 per night, 400 cleaning
- **Category B**: 800 per night, 350 cleaning
- **Category C**: 600 per night, 350 cleaning
- **Category D**: 550 per night, 150 cleaning
- **Category E**: 500 per night, 150 cleaning
- **Category F**: 450 per night, 150 cleaning
- **Category G**: 350 per night, 150 cleaning

The hotel's losses from a booking cancellation include the cost of one night and one cleaning, adjusted by the seasonal coefficient.

The budget for developing the prediction system is 400,000. The model must recoup this investment during the test period by generating more revenue than the cost of development.

## Data Description
The `hotel_train` and `hotel_test` datasets contain the following columns:

- **id**: Record number
- **adults**: Number of adult guests
- **arrival_date_year**: Year of arrival
- **arrival_date_month**: Month of arrival
- **arrival_date_week_number**: Week number of arrival
- **arrival_date_day_of_month**: Day of arrival
- **babies**: Number of infants
- **booking_changes**: Number of booking modifications
- **children**: Number of children (ages 3-14)
- **country**: Guest nationality
- **customer_type**: Type of customer (Contract, Group, Transient, Transient-party)
- **days_in_waiting_list**: Days waiting for booking confirmation
- **distribution_channel**: Booking distribution channel
- **is_canceled**: Booking cancellation flag
- **is_repeated_guest**: Repeated guest flag
- **lead_time**: Days between booking and arrival
- **meal**: Meal options (SC, BB, HB, FB)
- **previous_bookings_not_canceled**: Number of previous confirmed bookings
- **previous_cancellations**: Number of previous cancellations
- **required_car_parking_spaces**: Parking space requirement
- **reserved_room_type**: Reserved room type
- **stays_in_weekend_nights**: Number of weekend nights
- **stays_in_week_nights**: Number of weekday nights
- **total_nights**: Total number of nights
- **total_of_special_requests**: Number of special requests
