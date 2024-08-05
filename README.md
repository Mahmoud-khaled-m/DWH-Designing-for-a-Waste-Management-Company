# DWH-Designing-for-a-Waste-Management-Company
This project is designed to provide hands-on experience in designing, implementing, and querying a data warehouse using PostgreSQL. It simulates a real-world scenario where you, as a data engineer, assist a waste management company in Brazil.

## Problem Statement
You are a data engineer hired by a solid waste management company that collects and recycles solid waste across major cities in Brazil. The company operates hundreds of trucks of different types to collect and transport solid waste. They need a data warehouse to generate reports on various metrics such as total waste collected per year, per city, per truck type, and more.

### Project Steps

#### Exercise 1: Design a Data Warehouse
1. Designed the Star Schema:
   * Fact Table: MyFactTrips
   * Dimension Tables: MyDimDate, MyDimWaste, MyDimZone
2. Identified Fields:
   * Defined the fields for each table to capture the required data granularity and relationships.

#### Exercise 2: Create Schema for Data Warehouse on PostgreSQL
1. Created the Database:
    * Set up a database named Project.
2. Created Tables:
    * Implemented the schema by creating tables MyDimDate, MyDimWaste, MyDimZone, and MyFactTrips in PostgreSQL.
      
#### Exercise 3: Load Data into the Data Warehouse
1. Adapted to New Data Requirements:
    * Due to operational changes, redefined the schema to include new tables: DimDate, DimTruck, DimStation, and FactTrips.
2. Created a New Database:
    * Set up a database named FinalProject.
3. Loaded Data:
    * Imported data from provided CSV files into the new tables: DimDate, DimTruck, DimStation, and FactTrips.
      
#### Exercise 4: Write Aggregation Queries and Create Materialized Views
1. Aggregation Queries:
    * Created queries using grouping sets, rollup, and cube to aggregate the data on various dimensions such as stationid, trucktype, city, and year.
2. Materialized View:
    * Created a materialized view to optimize query performance by precomputing and storing aggregated results.
