# Metricmind-Agentic-BI
### PROBLEM
giving an LLM direct access to a data warehouse causes SQL hallucinations and inconsistent metrics. Finance and sales see different numbers for the same metric like "Revenue".
### SOLUTION
MetricMind is an Agentic Semantic BI Engine. The LLM does not write raw SQL. It talks to a governed semantic Layer first. This ensures every answer users the exact same business logic and prevents wrong data.
## TECH STACK
-" Semantic Layer": cube.dev / dbt
-"Agentic AI" : Langchain,Llama 3 
-"Data warehouse" ; snowflake / databricks
-"UI":Next.js,Tremor , Echarts
##PROJECT GOAL
Build a production-ready conversational BI Tool that finance teams can trust 100%.


## PROGRESS LOG
#### DAY 1-JULY 14
- Create GitHub repository
- Updated README  file with problem,solution,Tech stack
- Defined project scope 
#### DAY 2 -JULY 15
- Download superstore sales Dataset from kaggle
- Analyzed sales by category in Excel
- Analyzed profit by category in Excel
- created charts for data visulization
- uploaded Excel file:[Excel_assigment.xlsx](Excel_assigment.xlsx)
### DAY 3 JULY 17 - Snowflake Environment Setup
  - Created a Snowflake Trial account.
- Explored the Snowflake Snowsight interface.
- Created the METRICMIND_DB database.
- Created the SUPERSTORE table.
- Uploaded the Sample Superstore dataset into Snowflake.
- Verified that the data was loaded successfully.
- Executed basic SQL queries:
  - SELECT * FROM SUPERSTORE LIMIT 10;
  - SELECT COUNT(*);
  - SUM(SALES), SUM(PROFIT);
  - COUNT(DISTINCT ORDER_ID);
- Fixed table schema and data loading issues.
  ### DAY 4 JULY 18 - dbt Setup and Snowflake Connection
  - Installed dbt Core
  - Installed dbt Snowflake adapter
 - Verified dbt installation
  ### DAY 5 JULY 20
- Completed dbt staging and cleaning models
- Verified 9,994 records
- Performed business analysis using Snowflake SQL
- Created KPI summary for Total Orders, Customers, Sales, Profit, Discount, and Quantity
  ### DAY 6 JULY 21
- Set up the Cube project for the MetricMind analytics platform.
- Installed and configured Cube CLI.
- Installed the Snowflake driver.
- Configured Snowflake database, schema, warehouse, and account details.
- Started the Cube development server.
- Identified and worked on the Snowflake connection configuration issue.
  ### DAY 7 JULY 22
- Created Cube.js project.
- Configured Snowflake account details.
- Added database, warehouse and schema configuration.
- Verified project folder structure.
- Tested Cube.js server startup.
- Identified initial connection issues.
  ### DAY 8 JULY 23
- Installed required npm packages.
- Updated Cube.js configuration.
- Resolved package installation issues.
- Verified Node.js and npm environment.
- Tested Cube.js development server.
- ### DAY 9 JULY 24
## Work Completed
- Connected Cube.js with Snowflake.
- Generated the `SUPERSTORE_CLEAN` schema.
- Verified dimensions and measures.
- Validated the data model in Cube Playground.
- Tested Cube.js queries.
- Prepared the backend for React integration.
- ## Status
 Cube.js Backend Ready
- ### Day 10 JULY 27
- Superstore Sales Dashboard Development
## Work Completed
- Created Superstore Sales Dashboard using React.
- Designed KPI Cards:
  - Total Sales
  - Total Orders
  - Categories
- Developed dashboard charts:
  - Orders by Category
  - Sales by Region
  - Sales by Segment
  - Profit by Category
  - Sales Trend by Year
- Fixed JSX syntax errors.
- Fixed React rendering issues.
- Successfully displayed dashboard in browser.
- Configured Cube.js client.
- Verified Cube.js server is running.
- Opened Cube Playground.
- Generated SUPERSTORE_CLEAN schema.
- Started Cube.js integration with React.
## Problems Faced
- JSX syntax errors.
- Blank dashboard.
- Cube.js integration issues.
- React rendering problems.
## Solution
- Corrected JSX syntax.
- Fixed rendering issues.
- Restored dashboard successfully.
- Verified Cube.js server and Playground.
## Status
- Dashboard UI Completed 
- Charts Completed 
- Cube.js Configured 
- Live Data Integration In Progress 
   ### DAY 11 JULY 28
- Connected React frontend with Cube.js
- Configured Cube API integration
- Displayed live Total Orders from Snowflake
- Implemented Orders by Category bar chart using Recharts
- Fixed React JSX and rendering issues
- Verified dashboard functionality in the local development environment
- 
  ### DAY 12 JULY 29
 - Refactored the React dashboard code structure
- Fixed JSX rendering and component issues
- Added KPI cards for Total Sales, Total Orders, and Categories
- Implemented Orders by Category visualization
- Added Sales by Region, Sales by Segment, Profit by Category, and Sales Trend charts
- Improved dashboard UI layout and responsiveness
- Tested the dashboard successfully in the local development environment

  ### DAY 13 AUG 3
Verified Git repository status using git status.
Verified remote repository configuration using git remote -v.
Investigated GitHub authentication issue during git push.
Diagnosed Git Credential Manager using git credential-manager diagnose (all checks passed).
Identified system-level credential.helper=manager configuration causing browser OAuth issues.
Removed system credential helper configuration with administrator privileges.
Configured Git to use credential.helper=store.
Successfully switched authentication flow from browser OAuth to terminal username/password prompt.
Began configuring GitHub Personal Access Token (PAT) authentication for secure repository access.
Status:
Repository configuration is correct.
Authentication flow is fixed up to terminal login.
Remaining task: complete GitHub authentication using a valid PAT and push changes successfully.

