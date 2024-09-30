---
date: "2024-09-30"
location: 
  - JCU courses/CP1401 - Programming/
hubs: 
    - "[[programming|Programming]]"
urls:
    - 
---

# Decision Structures
# Evaluate algorithms before coding them
+ WHAT SHOULD IT DO ?== WHAT DOES IT DO
-> Dont implement if they dont match -> using test values for "known for sure" results

# Correct and improve algorithms
+ Doesnt work:
    + Why? How to fix?
        1. Incorrect / Missing steps ?
        2. Steps in wrong place ?
        3. Typos? Incosistency?
+ Does work:
    + Improvement?
        1. Any unnecessary steps?
        2. More efficient / readable ?


# Test code
+ WHY? -> check if implemeneted solution correctly
+ Errors -> READ em
+ Make unclear -> familiarize

+ What to look for:
    + No syntax error
    + Correct results -> no logic errors
    + Special case inputs -> break program

# Logic errors
+ How to identify?
    + Test systematically
    + Incorrect results -> logic errors
    + Good test data?
        + KNOWN results
        + Represetative sample 
    + How to locate? -> debugging
    + How to fix? -> modify code or origial algo

# Look for decisions during problem decomposition
+ What words indicate decisions?
    + Conditional words (if. then, otherwise, else) -> represent decisions / repetitions
+ Read description carefully 
![[Pasted image 20240930151743.png]]
=> No repetition -> decision type
![[Pasted image 20240930151946.png]]

## Python requires proper indetation
> else aligned with if , satements be consistently indented


# Boolean variable names -> sound like actual bolean
+ is_..., will_...

# Test decisions systematically 
+ Test all possible paths in a decision statement
+ Examine conditions
+ Check for compund boolean exporessions -> many possible outcomes
+ Test unexpected values (within reason)
+ Representative sample is enoguh, dont need all
# Example of testing an algorithm
![[Pasted image 20240930153311.png]]
We need at least 3 ->
![[Pasted image 20240930153401.png]]
