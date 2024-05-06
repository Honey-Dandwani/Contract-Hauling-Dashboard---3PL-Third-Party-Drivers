### Contract Hauling Dashboard
 The contract hauling project aims to optimize transportation logistics and resource allocation for the efficient delivery of goods and materials. It involves managing and coordinating transportation contracts, routes, and carriers to ensure timely and cost-effective delivery while minimizing operational risks and expenses. Leveraging data-driven approaches and advanced analytics, the project focuses on improving route planning, load optimization, and fleet management to enhance overall supply chain performance and customer satisfaction.
 ![Dashboard](https://github.com/mlmariscotes/Fleet-Management-Dashboard/assets/99033220/4e12c5a4-8bbe-4094-b02c-820c4e5005de)

Typical Data Columns:

Shipment Information:
Shipment ID
Shipment Date
Origin Location
Destination Location
Quantity of Goods/Volume 
Type of Goods
Carrier and Vehicle Details:
Carrier ID
Carrier Name
Route and Distance Information:
Route ID
Origin Address
Destination Address
Distance between Locations
Estimated Travel Time
Route Optimization Parameters
Contract and Pricing Details:
Contract ID
Contract Terms
Pricing Structure
Billing Information
Payment Terms
Performance Metrics:
Cost per Shipment
Efficiency Metrics (e.g., Miles per Gallon, Cost per Mile)/
Line Haul Rate
Fuel Surcharge Rate
Operational Data:
Fuel Consumption
Maintenance Records
Driver Hours and Logs
Incident Reports
Customer and Order Information:
Customer ID
Customer Name
Order ID
Order Details
Actuals Data
Historical Data
Plan for current year
Number of Runs
Route Category

Contract Hauling SOP :

1. Contract Hauling
Contract hauling refers to the transportation of goods or materials by third-party carriers or contractors under a mutually agreed contract. These contracts specify terms and conditions for the transportation services, including routes, schedules, pricing, and service level agreements.
The goal of contract hauling is to move products efficiently and cost effectively from one location to another while maintaining service quality and compliance with safety and regulatory standards.
2. Purpose
This SOP serves to provide a step-by-step guide for maintaining and updating the Contract Hauling Dashboard in Power Bl. It is essential to ensure that the planning team, sales management, and executives can access critical insights into Contract Hauling, including Routes, Carrier Comparison, and Driver Performance. The dashboard, sourced from Consolidated files for 2022 and 2023, is updated at the close of each perjod to support the Contract Hauling project's mission of optimizing transportation efficiency, cost management, and performance measurement.
3. Scope
This SOP applies to the Power Bi Analyst responsible for updating and maintaining the Fully Loaded MC Dashboard at Pepsi Bottling Ventures.
4. Contributors
Danielle Graman, Dirk Phillips, Billy Walters
5. Stakeholders & customers:
Danielle Graman, Valerie Gallagher, Dirk Phillips, Billy Walters, Scott Bell
6. Responsibilities
   
The Power BI Analyst is responsible for:

﻿﻿﻿Collecting data from various sources (SQL, Access DB, and Excel).
﻿﻿﻿Updating and maintaining the Fully Loaded Models Dashboard in Power BI.
﻿﻿﻿Publishing the dashboard in Power BI service.
﻿﻿﻿Ensuring the security, accuracy, and timeliness of the data in the dashboard.
﻿﻿﻿Troubleshooting and resolving dashboard issues with dashboard functionalities.
﻿﻿﻿Monitoring industry trends ahd Power BI advancements in features and functionalities.
﻿﻿﻿Providing training and support to end-users.



Measures guide:


PY Miles:
﻿﻿Calculate the total miles for Previous year (2022).
﻿﻿PY Miles = Filter(year), Total Miles
Miles vs PY (growth%):
Find the growth percentage.
• Growth = miles2023/miles2022 - 1, 0
CY Runs:
: Callate the number of us for the curent year (2023).
PY Runs:
Calculate the number of runs for the Previous year (2022)
• PY Runs = Filter(year), Number of Runs
Runs vs PY (growth%):
Find the growth percentage.
Growth = Runs2023/Runs2022 - 1, 0
CY Line Haul Rate:
Calculate the average line haul rate for the current year (2023).
CY line haul rate - filter(year), Line haul rate
PY Line Haul Rate:
Calculate the average line haul rate for the current year (2023).
• PY line haul rate - filter(year), Line haul rate
Average Line Haul Rate vs PY (growth %):
Find the growth percentage.
• Growth -Line Haul Rate 2023 - Line Haul Rate 2022/ Line Haul Rate 2022
CY Volume 2023:
: Cal vote the Vo me fer the, Vent year (2023).

PY Volume 2022:
Calculate the Volume for the Previous year (2023).
: PY Volume 2022 - filter(year), Volume
Volume vs PY (Growth %):
• Find the growth percentage. Growth = Volume 2023 - Volume 2022 / Volume 2022
Rate/Mile:
﻿﻿Find the rate per mile.
﻿﻿Rate per mile = Line haul rate/Miles
Cost per Mile:
﻿﻿Calculate the cost per mile.
﻿﻿Cost Per mile = Total Expense/Miles
Miles/Run:
: Clear the miles peumber of Runs
YTD Miles:
: Caulie year-o-date mi-year && Filter/period) = Period, IF (Selected year = year. Lotal
miles 2022], [total miles 2023]
YOY Miles%:
Calculate the year-over-year growth percentage in miles.
YOY miles (%) = 2023Miles/2022 Miles - 1.0
Runs Mix (%):
• Calculate the mix of runs based on specific criteria.
Cost per Mile:
Calculate the cost per mile.
Cost Per mile = Total Expense/Miles
Miles/Run:
Calculate the miles per run.
Miles per run = Miles/Number of Runs
YTD Miles:
Calculate year-to-date miles.
YTD Miles = Filter(year) = year && Filter(period) = Period, If (Selected year = year. [total
miles 2022], [total miles 2023]
YOY Miles%:
Calculate the year-over-year growth percentage in miles.
YOY miles (%) = 2023Miles/2022 Miles -1,0
Runs Mix (%):
Calculate the mix of runs based on specific criteria.
Runs Mix - filter (price type),2023Number of runs /total number of runs + Filter (price type),2022Number of runs /total number of runs
Better Worse B/(W) (%):
Calculate the Better Worse based on specific criteria.
• B/(W)%= Plan total expense - Actual total Expense


Contract Hauling Dashboard Vocabulary:

CY - Current year
PY - Previous year
Runs - This refers to the number of trips or journeys made by a carrier to transport goods from one location to another. It indicates how many times the carrier has completed the transportation service.
Line Haul Rate - The line haul rate is the price or cost associated with the actual transportation of goods.
It often excludes additional charges such as fuel surcharges or accessorial fees.
Fuel Surcharge - A fuel surcharge is an additional fee or rate adjustment that carriers may charge to compensate for fluctuations in fuel prices. It helps carriers cover the increased cost of fuel.
Total Expense - This is the overall cost incurred by the carrier for providing transportation services. It typically includes line haul rates, fuel surcharges, and any other associated costs.
Rate/mile - Rate per mile is Line haul rate divided by miles.
Cost/mile - Cost per mile is Total Expense Divided by miles.
Runs Mix - Runs mix refers to the distribution or proportion of different types of transportation services, such as "power only" and "load on" runs, in the carrier's operations. It helps understand the mix of services provided.
Better worse — Better worse" is not a standard term, but in the context of your question, it might refer to a measure or calculation indicating whether the carrier's performance is better or worse compared to certain benchmarks or targets.
Carrier - A carrier is a company or entity responsible for transporting goods from one location to another.
Carriers can be trucking companies, logistics providers, or other entities involved in transportation. (BEST, BROWN, BARNES, EMERGE etc.)
Route Category - Route category could refer to the classification of transportation routes based on factors such as distance, geography, or specific service requirements. It helps in route planning and 
Runs - This refers to the number of trips or journeys made by a carrier to transport goods from one location to another. It indicates how many times the carrier has completed the transportation service.
Line Haul Rate — The line haul rate is the price or cost associated with the actual transportation of goods.
It often excludes additional charges such as fuel surcharges or accessorial fees.
Fuel Surcharge - A fuel surcharge is an additional fee or rate adjustment that carriers may charge to compensate for fluctuations in fuel prices. It helps carriers cover the increased cost of fuel.
Total Expense - This is the overall cost incurred by the carrier for providing transportation services. It typically includes line haul rates, fuel surcharges, and any other associated costs.
Rate/mile - Rate per mile is Line haul rate divided by miles.
Cost/mile - Cost per mile is Total Expense Divided by miles.
Runs Mix - Runs mix refers to the distribution or proportion of different types of transportation services, such as "power only" and "load on" runs, in the carrier's operations. It helps understand the mix of services provided.
Better worse — Better worse" is not a standard term, but in the context of your question, it might refer to a measure or calculation indicating whether the carrier's performance is better or worse compared to certain benchmarks or targets.
Carrier - A carrier is a company or entity responsible for transporting goods from one location to another.
Carriers can be trucking companies, logistics providers, or other entities involved in transportation. (BEST, BROWN, BARNES, EMERGE etc.)
Route Category - Route category could refer to the classification of transportation routes based on factors such as distance, geography, or specific service requirements. It helps in route planning and optimization. (Carolina Delmarva, intra Carolina, intra Delmarva, store delivery etc.)
Price type — These are different pricing models or types used in contract hauling. "Load On" and "Power Only" could represent different methods of pricing transportation services, depending on whether the carrier is responsible for loading goods onto the vehicles.
Destination Location - Customers Location like e.g. (Sams DC, Sams DC 6789)
Fuel Surcharge - A fuel surcharge is an additional fee or rate adjustment that carriers may charge to compensate for fluctuations in fuel prices. It helps carriers cover the increased cost of fuel.
Total Expense - This is the overall cost incurred by the carrier for providing transportation services. It typically includes line haul rates, fuel surcharges, and any other associated costs.
Rate/mile - Rate per mile is Line haul rate divided by miles.
Cost/mile - Cost per mile is Total Expense Divided by miles.
Runs Mix - Runs mix refers to the distribution or proportion of different types of transportation services, such as "power only" and "load on" runs, in the carrier's operations. It helps understand the mix of services provided.
Better worse - Better worse" is not a standard term, but in the context of your question, it might refer to a measure or calculation indicating whether the carrier's performance is better or worse compared to certain benchmarks or targets.
Carrier - A carrier is a company or entity responsible for transporting goods from one location to another.
Carriers can be trucking companies, logistics providers, or other entities involved in transportation. (BEST, BROWN, BARNES, EMERGE etc.)
Route Category - Route category could refer to the classification of transportation routes based on factors such as distance, geography, or specific service requirements. It helps in route planning and optimization. (Carolina Delmarva, intra Carolina, intra Delmarva, store delivery etc.)
Price type - These are different pricing models or types used in contract hauling. "Load On" and "Power Only" could represent different methods of pricing transportation services, depending on whether the carrier is responsible for loading goods onto the vehicles.
Destination Location - Customers Location like e.g. (Sams DC, Sams DC 6789)
Routes - In the context of contract hauling, "Routes" typically refers to the specific transportation routes or paths that carriers follow when transporting goods. The example you provided, such as "GAR-WIN" or
"GAR-WOW,"
represents specific routes or destinations. For example, e.g. (GAR -WIN, GAR-WOW)
Total Miles - Total Miles" is a measure of the cumulative distance traveled by the carrier during transportation. It's a critical metric for assessing the efficiency and cost-effectiveness of the hauling operations.
Period - In the context of Contract Hauling, "period" is likely referring to specific time intervals within a year, which can be used for various analytical and reporting purposes. These periods are often used to break down data and performance metrics into manageable segments for analysis. In your case, you have periods labeled from "p1" to "p13," which suggests there are 13 periods within a year.
Actual Shipping Period - It shows period and year together (P1 2023).
DSD Sales Volume - It refers to the quantity or amount of goods, products, or materials being transported. It represents the total cargo or load being moved from one location to another.


