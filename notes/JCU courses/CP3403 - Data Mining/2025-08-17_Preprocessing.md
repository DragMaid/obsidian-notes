---
date: "2025-08-17"
location: 
    - JCU courses/CP3403 - Data Mining
hubs: 
    - "[[]]"
urls:
    - 
---

# Preprocessing

## Reasons to preprocess
+ Noisy (has errors: age = -5)
+ Incomplete (missing values: age = None)
+ Inconsistent (different formats: age = 23, age = 1990)
=> Must have quality data to get quality mining results

## Data Cleaning
+ Number one problem in data warehousing
### Methods
+ Fill missing
+ Smooth noise
+ Identify / Remove outliers
+ Resolve inconsistencies
+ Resolve redundancy

### Handle missing data
+ Ignore the record
+ Fill missing manually
+ Fill automatically (mean, global constant, most probable value)

### Handle noisy data
+ Binning (sort data / partition into equal frequency bins) -> can smooth by bin means / boundaries / etc
+ Regression
+ Clustering (detect / remove outliers)
+ Combined computer + human inspection

## Data Integration
+ Combine many datasets into same format
+ Will need to resolve data conflicts & inconsistencies

## Data Transformation
+ Required mostly to suit the requirements of the DM algorithm
+ **Smoothing**: remove noise from data
+ **Aggregation**: summarization, data cube construction
+ **Generalization**: concept hierarchy climbing
+ **Attribute / Feature construction**: new attributes constructed from given ones
+ **Normalization**: scaled to fall within small specified range (min-max norm / z-score norm (standardization))
=> In short: **SAGAN**


## Data Reduction
+ Concept: Reduce size / dimension of data - but still produce same analytical results
+ **Data sampling**: selecting a representive subset of the data (horizontal reduction)
+ **Data compression**: transforming data into another format lossy (jpeg) or lossless (gif) 
+ **Generalization**: selecting the hierarchy (city - town - district - etc)
+ **Dicretisation**: Division of continuous values into intervals
+ **Dimensionality / Attribute reduction**: vertical reduction
+ **Data cube aggregation**: drill-down and roll-up in data warehouse


### [[Data Attribute Types]]

### Heuristic Feature selection methods
+ Independence assumption (by significance tests)
+ Best step-wise feature selection (pick best)
+ Step-wise feature elimination (remove worst)
+ Ugly-duckling theorem (there will always be bias)

### Data Dimension Reduction 
+ Reduce redundancy implied amog attributes
+ The bads: more dimension - more redundancy - more processing time - more complexity
+ How fix:
    + Linear algebra techniques:
        + [[Principle Component Analysis (PCA)]]
        + [[Independent Component Analysis (ICA)]]
        + [[Single Value Decomposition (SVD)]]
    + [[#Heuristic Feature selection methods]]
