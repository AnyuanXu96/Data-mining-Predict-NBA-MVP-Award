# Data-mining-Predict-NBA-MVP-Award
Predict the NBA most valuable player based on ML techniques

In this project, we aim to find a supervised machine learning algorithm which can predict 
the NBA's MVP winner with the highest accuracy and use this algorithm to predict the 
MVP winner for the current season.

# The goal of this project
Our goal is to find a supervised machine learning algorithm which can predict the MVP
winner with the highest accuracy and use this algorithm to predict the MVP winner for the 
current season

# The solution
1. Find the attributes regarding the players in the candidate list and obtain our data set. All 
the records from the dataset come from https://www.basketball-reference.com.
2. Perform data exploration, visualization, preparation, and preprocessing.
3. For this prediction problem, implement all machine learning algorithms which we have 
learned and can be used for the prediction problem on the training dataset and fit the model 
respectively.
4. Evaluate the performance on the validation dataset and select the algorithm that has the 
highest accuracy

# Data Exploration and Visualization
As we can see in the Figure 1, our data set consists of 412 observations and 23 variables. 
All the variables excepted the player's and team's name are numerical variable, thus there 
is no categorical variables.
For the 412 observations, they contain top 10 NBA MVP candidates in 40 seasons from 
1979-1980 season to 2019-2020 season, and we select past 40 years records because an 
important attribute: the 3-point was introduced in 1979-1980 season.
For the 23 variables, they include the attribute of MVP votes, team performance, player 
individual performance and individual advanced data. Apparently, the variable named 
"Share" is our outcome variable (aka response) and it represent the percentage of votes. 
Other variables will be filtered to compose our input variables (aka predictors)

![1641511590(1)](https://user-images.githubusercontent.com/73874161/148466647-badccf1e-8dcb-4abf-8f8d-acb98b7085a9.png)

![1641511662(1)](https://user-images.githubusercontent.com/73874161/148466735-2679c8a0-0248-483a-86ad-85cb907b550b.png)

![1641511716(1)](https://user-images.githubusercontent.com/73874161/148466801-cfb2571e-4dd5-4628-9c75-51f57c0e66b0.png)

![1641511734(1)](https://user-images.githubusercontent.com/73874161/148466820-07e8c4fc-7751-456a-9904-cc038390eebc.png)

# Data Mining Techniques and Implementation
The machine learning algorithms we used for our prediction problem are as follows.
1. Linear Regression
2. K Nearest Neighbors (k-NN) Regression
3. Regression Tree
4. Random Forests
5. Neural Network
6. Support Vector Regression (SVR)
We implement these data mining techniques on the datasets we obtained from both 
correlation analysis and PCA analysis. And the flow chart figure 10 is as follows.

![1641511814(1)](https://user-images.githubusercontent.com/73874161/148466919-5d766ba8-944d-4fb9-91a7-5455f692def8.png)

# Performance Evaluation
After we implement all algorithms on the training dataset and obtain the model respectively, 
we apply all models on the validation dataset to evaluate the performance by using lift chart 
and our accuracy list including RMSE and MAE, shown as figure 15 and table 2.

![1641511899(1)](https://user-images.githubusercontent.com/73874161/148467034-3cef3007-67ad-41db-b9b4-a0cc18ac3886.png)

![1641511917(1)](https://user-images.githubusercontent.com/73874161/148467060-f8dab4dd-feb8-4df6-8d1e-e424f376ab77.png)

![image](https://user-images.githubusercontent.com/73874161/148467083-0f245856-ffa0-40e5-bee0-f50fcb8cbff1.png)

# Discussion and Recommendation
According to the accuracy list and lift chart shown as figure 15 and table 2, we can find 
that linear regression, k-NN regression, neural network, and support vector regression
performs better than the tree model. The method which has the best performance is support vector regression (SVR). Finally, we will recommend that we can use the SVR method to predict the MVP for the 
current NBA season.

