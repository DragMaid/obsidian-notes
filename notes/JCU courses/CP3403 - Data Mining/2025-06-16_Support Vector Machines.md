---
date: "2025-06-16"
location: 
    - JCU courses/CP3403 - Data Mining
hubs: 
    - "[[]]"
urls:
    - 
---

# Support Vector Machines
+ Classification for both linear and non-linear data
+ Use non-linear mapping -> transform original data -> higher dimension
=> Search for linear optimal separating hyperlane (or decision boundary)
=> Linear mapping - sufficient high dimension - data from 2 classes can be separated by a hyperlane
=> Find hyperlane using support vectors (essential training tuples) and margins
![[Pasted image 20250616103306.png]]
** Caption: Original perceptron methods use multiple lines to separate
![[Pasted image 20250616103430.png]]
** Note: after SVM transform ori data into a higher dimension, data is clearly separable
![[Pasted image 20250616103516.png]]

# History and Applications
+ Training can be slow
+ Accuracy is high - model complex nonlinear decision boundaries (margin max)
+ Used for both classification and prediction
+ Application: everything that neural net do

# [[SVM vs Neural Network]]
