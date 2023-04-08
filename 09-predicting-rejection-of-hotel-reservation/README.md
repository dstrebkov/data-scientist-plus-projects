# Predicting rejection of hotel booking

## Data

Dataset contains the following information:

- `id` — record number;
- `adults` — number of adults;
- `arrival_date_year` — arrival year;
- `arrival_date_month` — arrival month;
- `arrival_date_week_number` — arrival week number;
- `arrival_date_day_of_month` — arrival day of month;
- `babies` — number of babies;
- `booking_changes` — number of booking parameter changes;
- `children` — number of children from 3 to 14 years old;
- `country` — guest citizenship;
- `customer_type` — customer type;
- `days_in_waiting_list` — how many days the booking waited for confirmation;
- `distribution_channel` — booking distribution channel;
- `is_canceled` — if the booking was cancelled or not;
- `is_repeated_guest` — a sign that the guest is booking a room for the second time;
- `lead_time` — number of days between booking date and arrival date;
- `meal` — booking options;
- `previous_bookings_not_canceled` — number of confirmed orders from the customer;
- `previous_cancellations` — number of canceled orders for a customer;
- `required_car_parking_spaces` — need for car parking space;
- `reserved_room_type` — type of room booked;
- `stays_in_weekend_nights` — number of nights on weekends;
- `stays_in_week_nights` — number of nights on weekdays;
- `total_nights` — total number of nights;
- `total_of_special_requests` — number of special marks.

## Task

To attract customers, a hotel company has added the ability to book a room without prepayment. However, if the client canceles the booking, then the company suffered money losses.

To solve this problem, it is needed to create a system that predicts hotel booking rejection. If the model shows that the booking will be cancelled, then the client is asked to make a deposit.

## Used Tools & Libraries
`pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`
