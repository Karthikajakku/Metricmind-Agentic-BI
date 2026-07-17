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
  - 
