# Homework #3 - Tabular Data

**Generate a large tabular dataset with 10 features, 1 regression target, 150 000 rows** 

 - I generated data similar to a real diabetes dataset. Dataset contains 10 features - symptoms and 1 target - the presence or absence of the disease. For this I used NumPy.
 - After that, I tried to build a relationship between the target and the features.
 - I also normalized the data by MinMax. The generated dataset looks like this:
 
![Screenshot (855)](https://user-images.githubusercontent.com/43314418/134784256-ba14c94f-0868-41a9-abe1-0a059d991582.png)

**Design Linear Regression (LR) as a benchmark**

- For X I used 3 columns: pedigree_function (the presence of the disease in relatives), glucose (sugar level), insulin (hormone). Analyzing the medical literature, I learned that these three indicators have the greatest impact on the presence of diabetes.
- For B, I used a target.
- I divided the data into training (80%) and test (20%). Then, using linear regression from the sklearn library, IS designed Linear Regression.
- The accuracy was 90%.

![Screenshot (857)](https://user-images.githubusercontent.com/43314418/134784571-57c13c95-b06f-48a2-b2c7-b36d6b014f56.png)
