# Brazilian E-commerce Risk & Performance Analysis

## Why I Built This
Working at Uber as a Risk and Compliance Specialist, I dealt with 
real business problems every day — fraud, cancellations, customer 
complaints, refund disputes. I wanted to apply that same risk 
thinking to e-commerce data and find the patterns that hurt 
businesses and the opportunities that drive growth.
This project analyses 99,441 real orders from Olist, a Brazilian 
e-commerce platform, to answer — where is the business losing money 
and where is it growing?

## Dataset
- Source: Olist Brazilian E-commerce Dataset (Kaggle)
- 99,441 real orders from 2016 to 2018
- 5 CSV files — orders, payments, reviews, customers, order items
  
## Business Questions Answered
1. How many orders were delivered late — and does it affect reviews?
2. Which states generate the most revenue?
3. Which payment methods dominate — and what risk does that create?
4. What are the monthly revenue trends?
5. What is driving 1 star reviews?
6. What is the cancellation rate — and is it linked to stock fraud?
7. How concentrated is revenue geographically — and what is the risk?

## Key Findings
**Delivery Performance**
6.61% of orders were delivered late, with a maximum delay of 188 days.
Late deliveries average 2.27 stars vs 4.29 for on-time orders — delivery 
directly drives customer satisfaction. Early deliveries raise expectations 
— when the same customer gets a late delivery later, frustration is higher.

**Revenue Concentration**
São Paulo generates 37.57% of total revenue. The top 3 states — SP, RJ, MG
— account for 63% of all revenue. This is a dangerous geographic 
concentration — if logistics in SP fail, the business loses over a third 
of revenue overnight.

**Cancellations and Stock Risk**
Cancellation rate is low at 0.63% (625 orders), but SP accounts for 55% 
of all cancellations despite generating 38% of revenue. 625 cancellations 
may be linked to 609 unavailable orders — sellers accepting orders without 
confirming stock availability. Recommendation: real-time inventory checks 
before order confirmation.

**Payment Fraud Risk**
74% of payments use credit card — the highest fraud risk payment method.
Customers may claim fraudulent transactions after receiving products
(chargeback fraud). Recommendation: 3-strike policy for refund claims
and real-time transaction monitoring.

**Review Score Distribution**
58% of customers gave 5 stars — but 11.5% gave 1 star. Customers either
love it or hate it, with very few in between. Late deliveries and wrong
or low quality items are the main drivers of 1 star ratings.

**Growth and Scale Risk**
Business grew 4,000x in revenue between 2016 and 2018. Rapid growth 
increases fraud and logistics risk if controls don't scale at the same pace.
Automated alert recommended — if late delivery rate exceeds 8%, trigger 
immediate logistics review.


## Tools
Python, Pandas, Matplotlib
