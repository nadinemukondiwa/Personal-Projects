# Analyzing flights to Harare

Author: Nadine Mukondiwa

Date: 23 February 2021

[TOC]

## Introduction

When I have travelled back home, I have always felt like the journey is very long and tiring. As a result, I was interested in analyzing the lengths of routes to Harare. I also wanted to estimate the average price of a flight in December 2022 based on flights' costs in December 2021.



Questions to Answer

* What is the distribution of prices?
* What is the distribution of flight duration (including the layover time)?
* What is the distribution of flight time?
* What is the distribution layover time?
* How many different stops does it take to get to Harare?

## Methodology

I created the dataset from data entry in Microsoft Excel based on the PDF file of round trip flights from Expedia. The flights had a departure date of 18 December 2021 and a return date of 1 January 2022.

For the data cleaning and data analysis, I used the Pandas library. I created different visualization using the seaborn library. 

Lastly, I carried out some statistical analysis of the correlation of different variables, hypothesis testing of the average price of flights. I generated a confidence interval to estimate the cost of flights in December 2022.

## Results

### What is the distribution of prices?

![chart](https://github.com/nadinemukondiwa/Personal-Projects/blob/main/Flights%20Analysis/images/price_distribution.png)

The lowest price of an economy flight is **$2626**, and the highest is **$3296**. Flights above **$3296** include mixed economy flights and other cabin types. Mixed economy flights are flights where one or more lags are in the premium economy cabin, which is much more expensive than the economy cabin.

### What is the distribution of flight duration (includes layover time)?

![chart](https://github.com/nadinemukondiwa/Personal-Projects/blob/main/Flights%20Analysis/images/flight_duration.png)

The flights' average duration (including layovers) is **1 day 17 hours and 8 minutes**. As seen in Chart 1 (appendix), Ethiopian Airlines has the least variability in flight duration.  Suppose one wanted to get to Harare as quickly as possible. In that case, the Ethiopian Airlines flight, Toronto- Addis Ababa - Harare, is the best. 

Interestingly, the flight with the longest total flight duration is not the one with the most stops. The longest flight duration is the British Airways flight with stops in London (Heathrow) and Johannesburg. 

### What is the distribution of flight time?

![chart](https://github.com/nadinemukondiwa/Personal-Projects/blob/main/Flights%20Analysis/images/flight_time.png)

In this, project flying time reference to the time spent on the airplane. The average flying time is  **20 hours and 6 minutes**. As mentioned above, the Ethiopian Airlines flight, Toronto- Addis Ababa - Harare, is the quickest way to get to Harare. The total flight time for that flight is **16 hours and 30 minutes**.

The longest flight time is an Emirate flight. The longest flight has three stops, with the first in London (Gatwick), then Dubai and finally Lusaka. The total flight time for that flight is **22 hours and 25 minutes**. 

### What is the distribution of layover time?

![chart](https://github.com/nadinemukondiwa/Personal-Projects/blob/main/Flights%20Analysis/images/total_layover_time.png)

The average layover time is **21 hours 2 minutes**. The Ethiopian Airlines flight mentioned above has the least layover time of **1 hour and 45 minutes**.  A British Airways flight with stops in London (Heathrow) and Johannesburg has the longest layover time of **1 day and 14 hours**.

### How many different stops does it take to get to Harare?

The minimum number of stops is one through Addis Ababa with Ethiopian Airlines. It can take as many as four stops to get to Harare. The economy routes (in this dataset) with four stops are:

- Amsterdam (AMS), Paris (CDG), Nairobi (NBO), Lusaka (LUN)
- Paris, Amsterdam, Nairobi, Lusaka
- Montreal (YUL), Paris, Nairobi, Lusaka
- New York (JFK), Paris, Nairobi, Lusaka

![chart](https://github.com/nadinemukondiwa/Personal-Projects/blob/main/Flights%20Analysis/images/routes.png)

A reference, airport codes are in the appendix.

## Conclusion

The journey from Toronto to Harare feels very long, mainly due to layovers. The airlines available to get to Harare are Ethiopian Airlines, British Airways, Air France, KLM and Emirates or a combination of multiple tickets under different combinations of these airlines. 

Based on my guess of the average price of economy flights to Harare, I found that the average could not be **$3000**. However, with 95% confidence,  flights from Toronto to Harare in December 2022 could cost between **$2737.71** and **$2973.39** on average.

## Appendix

Chart 1

![chart](https://github.com/nadinemukondiwa/Personal-Projects/blob/main/Flights%20Analysis/images/airline_flight_duration.png)

Multiple includes tickets that are under more than one airline.



Airport Codes

![chart](https://github.com/nadinemukondiwa/Personal-Projects/blob/main/Flights%20Analysis/images/airport_codes.png)
