# Neural_Network_Charity_Analysis

## Overview of the analysis

This analysis was made with the help of Machine Learning and Neural Networks to create a binary classifier for the prediction of the success of applicants being funded by Alphabet Soup, a charitable organization. The dataset contains information of more than 30,000 organizations with distinct measures that help make a model to try and predict the behavior of the fund. 
The process for the creation of the model (4 attempts were made due to efficiency issues) was firstly the preprocessing of the data for the neural network. Then the model had to be compiled, trained and evaluated. Lastly, efforts were made to optimize the process to increase the accuracy. 

## Results

The target column of this study is IS_SUCCESSFUL and the model was built around that. For the preprocessing columns that were not relevant were dropped since they didn't belong to targets or features of the models. The columns EIN and NAME were dropped since they were not considered factors that affected the study. 

In the first attempt made (main model) a selection of 2 hidden layers and one outer model was made. The first layer had 80 neurons and the second 50 neurons, both with the "relu" activation. The outer layer has a "sigmoid" activation function. 

![image](https://user-images.githubusercontent.com/85911181/139303903-7f93fb57-d7bf-4f07-91ad-91d64d83af64.png)

This model had an accuracy of 72.48% which did not meet the 75% expectacion.

![image](https://user-images.githubusercontent.com/85911181/139304259-8bf754c2-dc0c-411b-a748-ff30c22df2e5.png)

The next three attempts were comprised of the following characteristics:

### Attempt 1

- 2 hidden layers (800 and 500 neurons) Both "relu" activation function.
- Outer Layer with "sigmoid" activation function
- Accuracy of 72.65
![image](https://user-images.githubusercontent.com/85911181/139305452-e8ad67f1-4c21-42c0-b21e-e794ad424da9.png)


### Attempt 2 

- 3 hidden layers (400, 200, 100 neurons). All "relu"
- Outer Layer with "sigmoid" activation function
- Accuracy of 72.61%
![image](https://user-images.githubusercontent.com/85911181/139305761-c5b5ad43-04a4-45d6-a647-7afa2264c33f.png)

### Attempt 3

- 4 hidden layers (150, 150, 325, 150). All "relu" except the third which was "tanh".
- Outer Layer with "sigmoid" activation function
- Accuracy of 72.36%
![image](https://user-images.githubusercontent.com/85911181/139307465-b3c41b35-602d-4482-bc91-22d323d60b79.png)

## Summary 

Overall, the model after trying to optimize it stayed relatively the same with scores close to 72.5%. This may mean many different things, it may be underfitted, overfitted, a combination or overall lacks more information from the data origin. In this case, to improve accuracy of the model a Random Forest classifier could have been used. This would improve accuracy because the random forest classifier is a very accurate models that counts with an enough number of estimators and tree depth. This could also avoid an overfitting of data to improve overall efficiency and accuracy of the model. 



