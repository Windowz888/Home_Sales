# Home_Sales
SparkSQL Home Sales Analysis: In this challenge, we use SparkSQL to analyze a dataset of home sales. Our primary purpose is to obtain critical sales KPIs. This procedure includes the establishment of temporary views, data partitioning, table caching and uncaching, and cache status checking.

 Begin by establishing a new repository called Home_Sales for this project. It is not suggested that this task be merged with any existing repository. Clone this new repository to your local workstation and commit any changes you make to GitHub.

Files: You'll need some beginning files for this assignment. You can begin the challenge by downloading the following files: Module 22 Challenge files (link to follow).

Instructions: To begin, rename the file Home_Sales_starter_code.ipynb to Home_Sales.ipynb. Import the PySpark SQL functions required for this assignment next. Load the home_sales_revised.csv data into a Spark DataFrame and build the home_sales temporary table. Use SparkSQL to answer the following queries with this configuration:

Determine the annual average price of a four-bedroom house, rounded to two decimal places.
Find the average price of three-bedroom, three-bathroom homes built each year, again rounding to two decimal places.
Calculate the average price of three-bedroom, three-bathroom, two-story homes with at least 2,000 square feet built per year. Round your answer to the nearest two decimal places.
Determine the "view" grade for residences priced at $350,000 or above. Take note of the query's runtime as well, rounding your answer to two decimal places.
After gathering this information, cache the home_sales temporary table and check its caching status. Filter out view ratings for residences with an average price of $350,000 or higher using the cached data. Note the runtime and compare it to the runtime when the data was not cached. The data should then be partitioned depending on the "date_built" field and saved in parquet format. Create a temporary table for this parquet data and repeat the query, comparing the runtime. Finally, using PySpark, uncache the home_sales temporary table and validate its uncaching status. Finally, download and upload the Home_Sales.ipynb file to your "Home_Sales" GitHub project.
