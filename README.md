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



Measures:


PY Miles: Calculate the total miles for Previous year (2022).

PY Miles = Filter(year), Total Miles

Miles vs PY (growth%): Find the growth percentage.

Growth = miles2023/miles2022 - 1, 0

CY Runs: Calculate the number of runs for the current year (2023).

PY Runs: Calculate the number of runs for the Previous year (2022).

PY Runs = Filter(year), Number of Runs

Runs vs PY (growth%): Find the growth percentage.

Growth = Runs2023/Runs2022 - 1, 0

CY Line Haul Rate: Calculate the average line haul rate for the current year (2023).

CY line haul rate = filter(year), Line haul rate

PY Line Haul Rate: Calculate the average line haul rate for the Previous year (2023).

PY line haul rate = filter(year), Line haul rate

Average Line Haul Rate vs PY (growth %): Find the growth percentage.

Growth -Line Haul Rate 2023 - Line Haul Rate 2022/ Line Haul Rate 2022

CY Volume 2023: Calculate the Volume for the Current year (2023).

PY Volume 2022: Calculate the Volume for the Previous year (2023).

PY Volume 2022 - filter(year), Volume

Volume vs PY (Growth %): Find the growth percentage.

Growth = Volume 2023 - Volume 2022 / Volume 2022

Rate/Mile: Find the rate per mile.

Rate per mile = Line haul rate/Miles

Cost per Mile: Calculate the cost per mile.

Cost Per mile = Total Expense/Miles

Miles/Run: Calculate the miles per run.

Miles per run = Miles/Number of Runs

YTD Miles: Calculate year-to-date miles.

YTD Miles = Filter(year) = year && Filter(period) = Period, If (Selected year = year. [total miles 2022], [total miles 2023]

YOY Miles%: Calculate the year-over-year growth percentage in miles.

YOY miles (%) = 2023Miles/2022 Miles - 1.0

Runs Mix (%): Calculate the mix of runs based on specific criteria.

Better Worse B/(W) (%): Calculate the Better Worse based on specific criteria.

B/(W)%= Plan total expense - Actual total Expense


Contract Hauling Dashboard Vocabulary:

CY: Current year
PY: Previous year
Runs: Number of trips or journeys made by a carrier to transport goods.
Line Haul Rate: Price or cost associated with the actual transportation of goods.
Fuel Surcharge: Additional fee or rate adjustment to compensate for fuel price fluctuations.
Total Expense: Overall cost incurred by the carrier for providing transportation services.
Rate/mile: Rate per mile calculated as Line haul rate divided by miles.
Cost/mile: Cost per mile calculated as Total Expense divided by miles.
Runs Mix: Distribution or proportion of different types of transportation services.
Carrier: Company or entity responsible for transporting goods.
Route Category: Classification of transportation routes based on distance, geography, or service requirements.
Price Type: Different pricing models or types used in contract hauling.
Destination Location: Customer's location.
Routes: Specific transportation routes or paths followed by carriers.
Actual Shipping Period: Period and year together.
DSD Sales Volume: Quantity or amount of goods being transported.
Period: Specific time intervals within a year.
