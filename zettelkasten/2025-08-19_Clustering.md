---
date: "2025-08-19"
location: 
    - CP3403
hubs: 
    - "[[]]"
urls:
    - 
---

# Clustering
 

## Binary data
+ Binary variables are either **symmetric** or **asymmetric**
+ **symmetric** if both of its states are equally valuable (Example: male and female)
+ **asymmetric** if not equally valuable (Example: disease is positive or negative - where false positive is not as critical as false negative error - you're gonna die bro)

## Contigency table for binary data
![[Pasted image 20250819101836.png]]
+ Simple matching coefficient (symmetric): (b+c) / (a+b+c+d) (b, c would be the mismatches between the 2)
+ Jaccard coefficient (asymmetric): (b+c) / (a+b+c) (many of the times 0 doesn't mean mismatch but rather missing information - if both person don't have sth -> that doesn't mean they are similar) => That's why we rmoved d here

## Nominal (categorical) data
+ A normal nominal variable
+ Can have more than 2 states: Green, Red, Purple
+ Method 1: Simple matching: d(i, j) = (p - m) / p 
where m is number of matches
where p is total of variables

+ Method 2: use large number of binary variables (Straight up list out Green, Red, Purple as attribute with binary values like Y or N)
![[Pasted image 20250819124414.png]]

## Ordinal data
+ Typically discrete or contiuous
+ Step 1: replace values with rank
+ Step 2: (Optional) normalize on to \[0,1\]
+ Step 3: Compute dissimilarity (Eucledian metric)
![[Pasted image 20250819125146.png]]
![[Pasted image 20250819125131.png]]

## Mixture data types
+ A database might have all 6 types of variables
![[Pasted image 20250819125238.png]]
![[Pasted image 20250819125306.png]]

## Clustering Approaches
+ [[Partitioning Clustering]]
+ [[Hierarcical Clustering]]

## Cluster Evaluation
+ Within Cluster Sum of Squares (WCSS)
+ Within Cluster Manhattan Distance (WCMD)
![[Pasted image 20250819140842.png]]
+ Goal of clustering -> minimize WCSS
    + K-Means approximate min of WCSS
    + K-Medians approximate min of WCMD

## Partitioning vs Hierarchical
### Partitioning
+ Single level
+ Need to specify K
+ Clusters cover **local optimal** solution
+ Generally fast
+ Sensitive to outliers
+ Hard to detect clusters of different sizes
+ Fail to discover clusters of arbitrary shape (non-convex)

### Hierarchical
+ Sequence of possible groupings
+ Gives out **Global optimal** solution (cause it adapts without k)
+ Requires large memory / computational resources
+ Less sensitive to outliers (except single-linkage)
+ Single-linkage can create non-ellipsoial shape (but there are still limits)
