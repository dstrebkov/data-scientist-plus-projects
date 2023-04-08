# Determination of a prospective tariff for a telecom company


## Data

Table `users` (information about clients/users):

- `user_id` — unique client ID;
- `first_name` — client first name;
- `last_name` — client last name;
- `age` — client age (in years);
- `reg_date` — tariff registration date (day, month, year);
- `churn_date` — date of termination of the tariff (if the value is omitted, then the tariff was still valid at the time of uploading the data);
- `city` — client's city of residence;
- `tarif` — tariff plan name.

Table `calls` (information about calls):

- `id` — unique call ID;
- `call_date` — date of call;
- `duration` — call duration in minutes;
- `user_id` — ID of the client who made the call.

Table `messages` (information about messages):

- `id` — unique message ID;
- `message_date` — date when message was sent;
- `user_id` — ID of the client who sent the message.

Table `internet` (information about internet-sessions):

- `id` — unique session ID;
- `mb_used` — amount of internet traffic spent per session (in Mb);
- `session_date` — internet session date;
- `user_id` — ID of the client.

Table `tariffs` (information about tariffs):

- `tariff_name` — name of the tariff;
- `rub_monthly_fee` — monthly subscription fee;
- `minutes_included` — the number of minutes of conversation per month included in the subscription fee;
- `messages_included` — number of messages per month included in the subscription fee;
- `mb_per_month_included` — the amount of Internet traffic included in the subscription fee (in Mb);
- `rub_per_minute` — the cost of a minute of conversation in excess of the tariff package (for example, if the tariff includes 100 minutes of calls per month, then 101-th minute and all following minutes will be charged);
- `rub_per_message` — the cost of sending a message in excess of the tariff package;
- `rub_per_gb` — the cost of an additional gigabyte of Internet traffic in excess of the tariff package.

## Task

Telecom company offers its clients two tariff plans: _"Smart"_ and _"Ultra"_. To adjust the advertising budget, the commercial department of the operator wants to understand which tariff brings more profit.
It is needed to conduct a preliminary analysis of tariff plans on a small sample of clients. Available data contains information about `500` clients, such as: who they are, where they are from, what tariff they use, how many calls and messages each sent in `2018`. The task is to analyze the behavior of customers and draw a conclusion - which tariff of the two is better.

## Used Tools & Libraries
`pandas`, `numpy`, `scipy`, `matplotlib`, `seaborn`
