---
date: "2025-08-18"
location: 
    - JCU courses/CP3403 - Data Mining
hubs: 
    - "[[]]"
urls:
    - 
---

# Constrain ARM
+ User flexibility: provides **constraints** on what to mine
+ System optimization: explore **constraints** for efficient mining - constraint based mining

## Types of rule constraints
1. [[#antimonotonic|antimonotonic]]
2. [[#antimonotonic|monotonic]]
3. [[#succinctness|succinct]]
4. [[#convertibility|Conconvertible]]
5. [[#convertibility|inconvertible]]

### antimonotonic 
+ when itemset violates constraint -> so does all its superset
    + condition <= v is **anti-monotone** (if itemset sum is already v then adding more will only increase the sum)  => All superset violate constraint
    + condition >= v is **not anti-monotone** => Supersets can still satisfy the requirements

### succinctness
+ all and only satisfied sets are enumerated
+ itemsets can be generated that satisfy rules before support count starts
+ once subset is generated - testing can be avoided
+ Example: min(item.price) > 500, max(S) < 120 => this is succinct (prune while checking all items - no need to form set first)
+ Example: average(S) > v, average(S) < v => not succinct (to know average - gotta form the set first)
=> Therefore we remove the pruning process - which means faster processing speed

### convertibility
+ If not (anti)monotonic / succinct then we can make it like so by changing the order of the elements inside the set (changine the order of the elements before the sets are formed - not changing the order of the sets)
+ Example: average(S) < 150 - neither antimonotonic or monotonic because avg can either goes up or down => But if we sort the order of elements from big to small (descending) then average will only become smaller => Thus this shit is now monotonic

