---
date: "2025-08-18"
location: 
    - JCU courses/CP3403 - Data Mining
hubs: 
    - "[[]]"
urls:
    - 
---

# Association-Rules-Mining-(ARM)
+ Definition: is finding frequent patterens in a data set
+ Finding inherent regularities (associations) from frequent itemsets (association rules) (what goes with what ?)
+ Other names: affinity / market basket / frequent pattern analysis

## Frequent pattern
+ Pattern that occurs frequently in a dataset - can be foundation for other mining tasks

## Itemsets
+ Definition: a set of items (k-itemset has k items)
 
## Association Rule
+ Definition: relationshup between 2 disjoint(no overlap) itemsets X and Y
+ Example: X => Y where X is **antecedent** (initial assumption) and Y is consequent 
+ Does not represent **casualty** or **correlation**
### Types:
+ Actionable
+ Trivial - information already known
+ Inexplicable - no explanation and does not suggest action

## Support
+ Definition: probability that transaction contains X and Y

## Confidence
+ Definition: conditional probability that a transaction that has X also has Y

## Downward closure property
+ Any subset of a frequent subset must be frequent

## ARM methods
+ [[Apriori]]
+ [[FP-Tree]]

## Various Association Rules
+ [[Mining multilevel association]]
+ [[Mining quantitative association]]
+ Mining interesting correlation patterns

## Interesting Measure: Lift
+ Just support and confidence can be misleading
+ For example: play basketball => eat cereal (40%, 66.7%) is misleading
the overall % of students eating cereal is 75% > 66.7% (its just the fact that students really like to play basketball and they also like to eat cereal doesn't mean that people who play basketball would likely eat cereal)
=> Solution: use lift to shows the correlation also

## [[Constrain ARM]]
