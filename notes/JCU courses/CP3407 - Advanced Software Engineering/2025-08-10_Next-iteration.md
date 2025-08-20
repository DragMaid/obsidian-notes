---
date: "2025-08-10"
location: 
    - JCU courses/CP3407 - Advanced Software Engineering
hubs: 
    - "[[]]"
urls:
    - 
---

# Next-iteration
+ Change - move next iteration - rebuild board - adjust story - NOW
+ Complete iteration work
    + Pass all tests
    + Satisfy customer
+ Plan next iteration 
    + user stories
    + velocity
    + burn down
    + bugs
    + "next" user stories (from last iter that got moved here)
+ Revise story and task estimate and team velocity


## Integrating others code into yours
+ Same process just different code
1. user stories
2. estimates
3. priorities

**Note**: be careful when deciding to reuse sth - assuming the code works

+ test your new code - compile everything
+ TRUST no one
+ it doesnt matter who wrote the code - your software - your responsibility
+ you without your process

## Fixing bugs
+ Talk to the customer about the problem
+ Borken code magnets:
6. create place in bug tracker for issue
3. organize source code into standrd folder structure
10. write build script
4. put code in repo
7. integrate code into CI config
5. write test simulating how you need to use software
9. file bugs for issues

**Might consider not to do immediately yet**
2. figure package compiled version to include in your stuff
1. what dependencies and the impact
8. document the code
11. run coverage report
12. get line count of code to estimate how log 
13. do security audit on code
14. use UML to reverse-engineer code and create class diagram

### Get things buildable
+ Make it built sucessfully first
+ Functionality is the focus  - only fix code to fix user stories
    + Figure out what functionality works ?
    
### Spike test to estimate
+ Take little time to work on code - see what can get done - extrapolate from that
+ One week to conduct spike test - before giving the proper estimation

2. Pick random sampling from tests that are failing
+ Try to fix those first - random - not easy to fix or really hard ones
=> Get the idea of what work to get things going

3. End of week - calculate bug fix rate
total bugs fixed / number of days in spike test

**Note**: we can't be sure  - does not give quantitative data
**Note**: team feeling matters - factor in confidence of your team

Beautiful code is nice / but tested and readable code is delivered on time
=> Real success is about delivering functionality, period 

## Pinning down dev process
+ A framework that should enable you to make quality software
+ Common trails:
    + Develop iteratively
    + Always evaluate and assess
    + Incorporate best practices
    + Incorporate best practices (process skepticism)
