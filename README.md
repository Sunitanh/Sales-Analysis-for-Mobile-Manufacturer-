# Sales-Analysis-for-Mobile-Manufacturer-
**Business Context:**
A mobile phone manufacturer wants to analyze historical sales data to better understand customer behavior, market trends, and product performance. This includes evaluating performance across different states, identifying top-performing models and manufacturers, tracking customer spending patterns, and uncovering new business opportunities based on sales insights from multiple years.
________________________________________
**Problem Statement:**

The company’s leadership needs clear, data-driven answers to strategic questions like:

•	Which manufacturers and models are selling well in specific regions?

•	Are there loyal, high-value customers who can be targeted?

•	How are sales trends evolving over years?

•	Which manufacturers are gaining or losing market share?

By analyzing this sales data stored in a relational database, the goal is to uncover patterns and actionable insights that will drive better marketing, production, and sales strategies.
________________________________________
**Data Availability:**
The data resides in a relational schema with the following key tables:

•	**Dim_Manufacturer:** Manufacturer details

•	**Dim_Model:** Model-level metadata including model name, manufacturer, price, etc.

•	**Dim_Customer:** Customer demographics

•	**Dim_Location:** Location details (state, ZIP code, etc.)

•	**Fact_Transactions:** Sales data including quantity, date, price, model ID, and customer ID
________________________________________
**Data Understanding:**
Each fact transaction links multiple dimensions:

•	Customer (who bought)

•	Location (where it was bought)

•	Model (what was bought)

•	Manufacturer (who made the model)

Date and price data are embedded in transactions, enabling time-series and financial analysis. Common business questions revolve around:

•	Temporal sales trends

•	Top products and brands

•	Customer loyalty and spend

•	Geographic performance

•	Product pricing insights
________________________________________
**Key Steps Performed:**

**1.	Schema Creation:**

o	Used the provided database creation file to generate schema structure.

o	Verified foreign key relationships and indexes for performance.

**2.	SQL Query Development:**

o	Wrote SQL queries between --BEGIN and --END blocks in the provided answer_template.sql.

o	Used aggregation functions, joins, window functions, GROUP BY, RANK(), and CASE statements for complex analysis.

**3.	Testing & Validation:**

o	Each query was tested using provided data to validate logic.

o	Ensured all outputs return a single result table, as per submission rules.

**4.	Finalization & Submission:**

o	Renamed the answer file with email ID format.

o	Zipped the .sql file as required.
________________________________________
**Technology Stack Used:**
•	SQL
________________________________________
**Key Outputs:**

•	States where mobile phones were sold since 2005

•	Top-performing states for Samsung sales

•	Most frequently sold models per zip code

•	Cheapest cellphone identified

•	Top 5 manufacturers by quantity and their model-wise average prices

•	High-value customers in 2009 with average spend > ₹500

•	Models that were top 5 across 2008, 2009, and 2010

•	Second-best manufacturers in sales for 2009 and 2010

•	Manufacturers active in 2010 but not 2009

•	Year-wise customer spend, quantity, and % change for top 100 customers
________________________________________
**Challenges & Learnings:**

**Challenges:**

•	Interpreting schema relationships without access to actual data

•	Handling date-based logic for multi-year comparisons

•	Using window functions and CTEs efficiently within SQL-only constraints

•	Ensuring all outputs adhered to the "one table only" rule

**Learnings:**

•	Deepened knowledge of advanced SQL concepts: window functions, subqueries, ranking

•	Learned to work with a simulated schema in absence of raw data

•	Improved skills in query optimization and logic structuring

•	Understood how to analyze customer value over time using only SQL
