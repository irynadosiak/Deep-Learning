# Homework #3 - Tabular Data

**Generate a large tabular dataset with 10 features, 1 regression target, 150 000 rows** 

 - I generated data similar to a real diabetes dataset. Dataset contains 10 features - symptoms and 1 target - chances of having diabetes. For this I used Faker.
 - After that, I tried to build a relationship between the target and the features. Analyzing the medical literature, I learned that some indicators have greater impact on the presence of diabetes.
 - I also scalered the data by MinMax. The generated dataset looks like this:
 
![Screenshot (894)](https://user-images.githubusercontent.com/43314418/135346562-0b3b3460-8522-4e74-a943-7d9dd03e7b88.png)

All features are independent of each other, and the target is dependent on features:

![Screenshot (895)](https://user-images.githubusercontent.com/43314418/135346996-c7b6c334-06bf-4c98-b4e0-fbd92af481a0.png)

**Design Linear Regression**

- For X I used all columns without target.
- For B, I used a target.
- I divided the data into training (80%) and test (20%). Then shuffled them and, using linear regression from the sklearn library, IS designed Linear Regression.
- The MSE was 0.006295969155164378.

**Design 3 Dense Neural Networks:**
- **(DNN1) with 1 hidden layer**
- **(DNN2) with 5 hidden layers**
- **(DNN3) with 25 hidden layers**

**Prepare 3 optimizers**:
- (OPT1) SGD
- (OPT2) RMSProp
- (OPT3) Adam

**Explore the following learning rates**:
- (lr1) 0.1
- (lr2) 0.01
- (lr3) 0.001
