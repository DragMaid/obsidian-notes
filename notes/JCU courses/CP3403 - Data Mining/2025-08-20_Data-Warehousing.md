---
date: "2025-08-20"
location: 
    - JCU courses/CP3403 - Data Mining
hubs: 
    - "[[]]"
urls:
    - 
---

# Data-Warehousing

## Database vs Data warehousing
### Database 
+ A structured set of data
+ Data structured for efficient Online Transaction Processing (OLTP)
+ ETL is relatively easy / real-time
+ Entity-Relationship modeling
+ Normalized
### Data Warehousing
+ A structured set of data
+ Data structured for effcient queries and analysis (OLAP)
+ ETL is relatively complex / in batches
+ Dimensional modeelling
+ Denormalized
![[Pasted image 20250820022746.png]]

## Definition
+ A decision support db maintained separately from operational db
+ Support information processing / platform of consolidated / historical data for analysis
+ It's [[#subject-oriented]], [[#Integrated]], [[#time-variant]], [[#nonvolatile]]

## Subject-oriented
+ Organize major subjects (customer, product, sales)
+ Focus on analysis of data for decision
+ Provide simple and consise view of subjects (excluding useless data)

## Integrated
+ Constructed by integrating from multiple sources
+ Data cleaning / integration techniques applied (ensure consistency in naming, encoding, etc)
+ When data is moved here, it is converted

## Time-variant
+ Time horizon is way longer than operational (past 5-10 years - historical)
+ Every key structure here as **Time element**

## Non-volatile
+ A physically separate store of data
+ Operational update of data does not transfer here
    + No need for transaction processing / recovery / etc
    + Requires only 2 operations: **initial loading of data** and **access of data**

## Extraction-Transformation-Loading (ETL)
+ Extracted from OLTP db
+ transformed to match data warehouse schema
+ loaded into data warehouse db
=> Requires periodic update (monthly / daily / hourly)

### Extractuion
+ Process of copying data from one to another db
+ Get data frommany sources

### Transformation
+ Changes data - provide guidance whether data can be used for intended purposes
+ Performed in staging data

### Loading
+ Designed to have minimal sets of components
+ Design surrogate keys - have meaningless unique interger for primary keys from dimensions
+ De-normalized flat fact tables

## Metadata
+ Stores description of structure of dwh: schema, dimensions, hierarchy, etc
+ Operational metadata
    - data lineage, currency, monitoring info

## Dimension Tables
+ Dimensions provide the "who, what, where, when, why, how"
+ Business entities
+ Descriptive attributes (typically textual)
+ Product (product_name, brand, type) or time(day, week, month, quarter, year)

## Fact table
+ Facts are measurements / metrics from business process event
+ Conains measures (prices) and key to each of realated dimension tables

![[Pasted image 20250820024742.png]]