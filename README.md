# Exploratory Data Analysis of NYC Taxi Operations from TLC Data 
## [Capstone 2 JCDS Purwadhika]

**Preface**

This project is created as an exercise and to complete my Capstone Module 2 Project of Data Science bootcamp in Purwadhika,
and also serves as a preview of my work and marks my learning journey of becoming a full fledged Data Scientist.

Feel free to give any feedbacks and reach out to me via [email](dwika.widyantama@gmail.com) or connect with me on [LinkedIn](www.linkedin.com/in/dwika-w/)

## Before you dive in
This project comprises of several part in different format:
1. [Jupyter Notebook](https://github.com/d-widyantama/Capstone2-Purwadhika/blob/main/V1-EDA-NYCTaxi.ipynb) for more detailed Exploratory Data Analysis 
2. [Tableau Story]() for Data Visualization and Analysis
3. [Tableau Dashboard]()
4. [Slides Format]()


## About The Project
---

# **Overview**
New York City Taxi and Limousine Commission (TLC) is the agency responsible
for licensing and regulating New York City's medallion (yellow) taxis, street hail livery (green) taxis,
for-hire vehicles (FHVs), commuter vans, and paratransit vehicles.

The Taxi and Limousine Commission (TLC) regulates how much a cab can charge per mile or per minute, determines a cab company's leasing fees for drivers, monitors routes taken by the drivers (to ensure they are not artificially inflating the price), and much more. In essence, a cab company (or a cab driver) can only make as much money as the government allows them to make. 
[Read more](https://www.investopedia.com/articles/professionals/092515/how-nycs-yellow-cab-works-and-makes-money.asp)

The taxis in New York are operating in NYC area which divided by 5 borough:
1. 'Manhattan'
2. 'Brooklyn'
3. 'Queens', 
4. 'Bronx',
5. 'Staten Island']

**For non New Yorkers:**
Boroughs (pronounced burrow) are formal subdivisions of cities that have some aspects of self-government.

The TLC collects trip record
information for each taxi and for-hire vehicle trip completed by our licensed drivers and vehicles.
We receive taxi trip data from the technology service providers (TSPs) that provide electronic
metering in each cab, **this data will be the base of our dataset** in our analysis.


## **Stakeholder Statement**

Taxi companies may be interested in understanding demand patterns, identifying popular pickup/drop-off locations, and pricing strategies to maximize revenue. They may also want to improve service quality and efficiency based on customer behavior analysis.

## **Goals Setting & Problem Statement**

    1. How to optimize revenues and streamlining operations?  
   
    2. How to to better serve customers by undertanding their behaviours?  
   
    3. How to optimize the distribution of drivers?

# What's covered in the analysis?

This project analysis generally aims to provide insights on the day-to-day operations of NYC taxi. Starting from a raw dataset that's been provided which includes the information about taxi trips collected from the taxis. In general, the steps done in the project will consists of:
1. Data Preparation
2. Data Cleaning
3. Adding Additional Data Features
4. Data Analysis
5. Conclusion & Key Findings
6. Reccomendations


# Dataset Glossary
### NYC TLC Taxi Trip Data

| Columns       | Description |  Notes| 
| :---          |    :----   | :---- | 
| 'VendorID'    | LPEP provider that provided the record.|  |
| 'lpep_pickup_datetime',   | Starting time from taxi meter
| 'lpep_dropoff_datetime',  | Ending time from taxi meter
| 'store_and_fwd_flag',     | Trip record are saved and send after signal received | Y= store n forwad N=Not store n forward  
| 'RatecodeID',             | The final rate code in effect at the end of the trip.   *There are different rates for different type of trips & airport destination.*|  1=Standard rate, 2=JFK (Airport rate), 3=Newark   (Newark Country), 4=Nassau or Westchester (County), 5=Negotiated fare , 6=Group ride|
| 'PULocationID',           | Pickup location, using Taxi Zone code
| 'DOLocationID',           | Dropoff location, using Taxi Zone code
| 'passenger_count',        | # of passengers, driver manually input, max 6 by law
| 'trip_distance',          | Distance per trip, in miles
| 'fare_amount',            | The time and distance fare is calculated by the meter. includes the $0.50 and $1 rush hour and overnight charges
| 'extra',                  | only includes the $0.50 and $1 rush hour and overnight charges.
| 'mta_tax',                | $0.50 MTA tax that is automatically triggered based on the metered rate in use.
| 'tip_amount',             | tips from customers, tips from customers with CC payment
| 'tolls_amount',           | tolls fare amount
| 'ehail_fee',              | - | unidentified, all nulls  **[TO BE DROPPED]** |
| 'improvement_surcharge',  | $0.30 improvement surcharge assessed on hailed trips at the flag drop.
| 'total_amount',           | The total amount charged to passengers. Does not include cash tips.
| 'payment_type',           | 1 = Credit card 2 = Cash 3 = No charge 4 = Dispute 5 = Unknown 6 = Voided trip
| 'trip_type',              | 1 = Street|hail (inside the city) 2 = Dispatch (outside city)
| 'congestion_surcharge'    | surcharge for traffic congestion

---
*This project is created by Dwika Widyantama / @d-widyantama*

Also find my other works here:
- Medium    : https://medium.com/@dwika.widyantama
- Tableau Public : https://public.tableau.com/app/profile/dwika.widyantama
