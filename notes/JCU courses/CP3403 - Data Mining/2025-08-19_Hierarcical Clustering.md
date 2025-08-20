---
date: "2025-08-19"
location: 
    - JCU courses/CP3403 - Data Mining
hubs: 
    - "[[]]"
urls:
    - 
---

# Hierarcical Clustering
+ Multi-level nested decompositions (quality clusters reveal hierarchy)
+ Use distance matrix as clustering data - no need for k - but needs termination condition

## Types
+ Bottom-up (**agglomerative**) (singleton to whole) [[AGNES]]
+ Top-down (**divisive**) (whole to singleton) [[DIANA]]

## Agglomerative vs Divisive
+ Agglomerative: faster 
+ Divise: gives better view on global structure at the beginning

## Criteria
+ One of the agglomeration method is to merge clusters with minimum distance
### Distance Calculation methods
+ **Single Link**: smallest distance between points 
    + Strength: can handle non-global shape
    + Weakness: sensitive to outliers and noise
+ **Complete Link**: largest distance between points
    + Strength: less affected by noise and outliers
    + Weakness: tend to break big clusters
+ **Average link**: averagge distance between all pair-wise points
    + Weakness: tend to break big clusters
+ **Centroid**: distance between centroids
    + Weakness: tend to break big clusters

![[Pasted image 20250819140248.png]]
