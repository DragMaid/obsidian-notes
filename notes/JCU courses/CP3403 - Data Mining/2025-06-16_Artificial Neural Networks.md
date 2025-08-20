---
date: "2025-06-16"
location: 
    - JCU courses/CP3403 - Data Mining
hubs: 
    - "[[]]"
urls:
    - 
---

# Artificial Neural Networks
+ Among most effective learning methods but also inefficient
+ Inspired by biological learning (via complex webs of interconnected neurons)
=> Try to capture this parallel computation

# Perceptrons
+ Definition: Basic unit of ANNs
+ Takes vector of real-valued inputs
+ Calc linear combination of inputs
+ Goes into transfer func (return 1 if result > threshold else -1)

![[Pasted image 20250616090218.png]]

# Limitation
+ One neuron set up a straight line decision boundary
=> Only works for linearly separable datasets
=> Solutions: just add more to the network [[multi-perceptron]]


# Multi-perceptron
![[Pasted image 20250616090512.png]]
+ Each perceptron has different weights
+ Output cam be copied to inputs of many

# Feed Forward Neural Networks
+ Multiple inputs and single layer
+ Multiple inputs and multiple layers
![[Pasted image 20250616090740.png]]

# Recurrent Neural Nets
+ Same as feed forward but (the outcome can become the input again)
![[Pasted image 20250616090847.png]]

# One hidden layer is enough
+ Why only feed-forward + one hidden layer ?
+ With enough neurons in the hidden layer -> can approximate any bounded func to whatever accuracy
    + Bounded = function does not go to inf
    + More neurons = more accuracy

# Goods
+ High tolerance to noisy data (because many iterations)
+ Can classify untrained patterns
+ Suited for continuous valued inputs and outputs (not just categorical)
+ Wide range application
+ Algorithm are parallel -> fast
+ Developed for extraction of rules from trained neural nets

# Bads
+ Long train time
+ No idea how many neurons needed (or how to connect)
+ Poor interpretability
    + Gives answer -> but no idea how it works -> should we trust it ?

# Issues
+ Num source nodes
+ Num hidden layers
+ Interconnections
+ Weights
+ Activation funcs
+ Learning techniques
+ When to stop learning

# Representation
+ Boolean func - represented by network - single hidden layer
+ Bounded continuous funcs -> approximated with arbitrary precision by a network with one / large hidden layer
+ Any func can be approximated to aribitray accuracy by a net with 2 hidden layers
+ Overfit if there are too mnay params compared to data avail

## Choosing number of hidden units
+ Too few -> no learn
+ Too many -> slow or overfit
+ If n inputs are binary -> logn is good choice
+ Choose num of layers
    + Always start with 1
    + Never go beyond 2 hidden layers


 
