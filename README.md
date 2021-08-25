# ModelSelection

In this repo i have:
- Clean the data
- Split the data into train, validation and test
- Fit an initial model and evaluate 
- Tune the hyperparameter
- Evaluate the data into validation 
- Select and evaluate final model on test set

<img width="1148" alt="final_model_selection" src="https://user-images.githubusercontent.com/70954565/130751628-a032795f-343f-4336-9fd6-57b156a2e210.png">

Titanic.ipynb file is the foundation. Cleaning the data and Spliting data into train, val and test was done in that file. Then i have created five models :
- Logistic Regression
- Support Vector Machines
- Multilayer Perceptron
- Random Forest
- Boosting

Below are the brief introduction for each model
- Logistic Regression
  
  Regression is a statistical process for estimating the relationships among variables. This is often used to make a prediction about some outcome. Linear regression is one type     of regression that is used when you have a continuous target variable. 

- Support Vector Machines
  
  Support vector machines is a classifier that finds an optimal hyperplane that maximizes the margin between two classes.
 
- MLP
  
  Multi-layer perceptron is a classic feed-forward artificial neural network. This is one of the core components of some deep learning algorithms. 

- RF
  
  A random forest is a machine learning technique that’s used to solve regression and classification problems. It utilizes ensemble learning, which is a technique that combines     many classifiers to provide solutions to complex problems.
  
- Boosting
  
  Boosting combines the weak learners to form a strong learner, where a weak learner defines a classifier slightly correlated with the actual classification. In contrast to a weak   learner, a strong learner is a classifier associated with the correct categories.
  
I have created five notebook for five model and train the model with the train data set and then i have found the best param or the best estimator for each model and best estimator was saved into json files of each model.

## Best Estimator of each model

![Capture](https://user-images.githubusercontent.com/70954565/130757259-faaece7d-159d-4ecb-81dc-e2eb6b412f3d.PNG)

## Comparision of algorithm

![Comparision](https://user-images.githubusercontent.com/70954565/130760067-132129dd-6efc-42b7-8933-eecf0eff3f33.PNG)

FinalModelSelection does this things :
- Evaluate all of our saved models on the validation set
- Select the best model based on performance on the validation set
- Evaluate that model on the holdout test set

## How does it

<img width="1080" alt="hyperparameters" src="https://user-images.githubusercontent.com/70954565/130761273-5d076621-c5a0-4a25-b30f-1d851f07a942.png">

Notes:
- I have used google colab and i have mounted my drive so all the path of the files are related to my drive. Please change if you are using in the locally or your colab
- titanic.csv is the dataset which is used in the machine learning 
