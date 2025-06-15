---
date: "2025-06-15"
location: 
    - JCU courses/CP3407 - Advanced Software Engineering
hubs: 
    - "[[]]"
urls:
    - 
---

# Good-enough-Design
## Summary
+ Bad desing -> hard for everyone -> learn to refactor -> helps team be productive and software more flexible
+ Apply [[principles of good design]]
+ Handle unplaneed tasks

** Note: well-designed classes are singularly focused
# [[2024-10-28_Single-Responsibility-Principal-]]

## Spotting Multiple Responsibilities in design
1. Template: The [blank] [blank] itself -> for every method in class
2. First blank of each line, write class name.
   Second blank, write one of the methods in class 
   Do this for every methods in class
3. Read each line out loud - (May need another letter / word to read normally)
=> Does what you just said make sense or not ? Does class has responsibility that the method indicate it has does ? => If not (SRP violated)

## Design must be SRP & DRY
### Ripple effect
+  When one small change cause ripple changes throughout your code
=> You also need to ensure DRY (Don't repeat yourself)
    + Avoid duplicate code by abstracting or separating things
    => Piece of info and behavior in sys in single, sensible place

** Note: Unplanned tasks are still just tasks

