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

**Design 3 Dense Neural Networks with 3 optimizers and three different learning rates:**
- **(DNN1) with 1 hidden layer**, **(DNN2) with 5 hidden layers**, **(DNN3) with 25 hidden layers**.
- **(OPT1) SGD**, **(OPT2) RMSProp**, **(OPT3) Adam**.
- **(lr1) 0.1**, **(lr2) 0.01**, **(lr3) 0.001**.

The results, namely MSE for all models, are saved in results.xlsx. They look like this:

![Screenshot (896)](https://user-images.githubusercontent.com/43314418/135447985-9afe644d-cd74-4d3e-aab9-a4f83190c414.png)

Learning curves plots are saved in results. Totally, there are 27 graphics.

**Conclusions:**
- **Optimizer**: Adam shows the best results. Moreover, it works best with a small learning rate. RMS shows good results for 1 layer, 0.01 learning rate and for 5 layers, 0.1 learning rate. As for SGD, it shows good results for 0.1 learning rate.
- **Learning rate**: If a learning rate is large, the neural network does not learn well. 
- **DNN architecture**: If there are many hidden layers, they can slow down training. If not enough, the accuracy may be low. For example, the result is the best for 5 layers. 1 layer is not enough, 25 is too much.
