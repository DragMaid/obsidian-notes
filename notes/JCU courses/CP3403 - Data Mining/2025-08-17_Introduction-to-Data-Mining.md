---
date: "2025-08-17"
location: 
    - JCU courses/CP3403 - Data Mining
hubs: 
    - "[[]]"
urls:
    - 
---

# Introduction-to-Data-Mining

## Definition
+ NVNPU (the secret spell)
+ Data Mining is a non-trivial process of identifying valid, novel, potentially useful, understandable patterns from big datasets
    + nontrivial: not a single simple computation
    + valid: pattern found is general not to apply to unseen data with accuracy
    + novel: pattern is unexpected, not obvious
    + potential useful: can translate to effective actions
    + understandable: simple, interpretable
=> fnding patterns / learning (inference) / exploratory 

## Opposite of data mining
+ Simple search and query processing
+ (Deductive) exert systems
+ Small Machine Learning

## Basic concepts
+ Induction - from specific to general (all humans are mortal -> socrate is human -> socrate is mortal)
+ Deduction - from general to specific (100 swans are white -> all swans white)
=> Deduction would often produce the least error rate (because it applies general rules to a specific case)
+ Abduction - inference to best explanation (grass wet -> probably rained)

## [[Knowledge Discovery (KDD)]]
## [[Business Intelligence]]
## Data Mining Techniques

### Descriptive Mining
- [[Clustering]]
+ [[Characterization]]: generalize data to find descriptions
+ [[Deviation Detection]]: finding outliers that deviate from aggregations
=> Description: characterization and discrimination

### Predictive Mining
+ [[2025-06-09_Classification|Classification]]
+ [[Trend Dectection]]
+ [[Association]]: finding interesting dependencies among attributes
=> Description: Trend and Evolution analysis (trend & deviation  sequential pattern mining / periodicity analysis) 

## Challange - Bottleneck
+ Volume: sheer amount of data
+ Variety: data coming from multiple formats (txt, videos, etc)
+ Velocity: speed of data generation / processing
+ Veracity: trustworthiness and quality of data

### Issues
+ Not all patterns ar interesting
+ Completeness (find **all** interesting patterns)
+ Optimization (find **only** interesting patterns)
