# Twitter Bot Detection (capstone)
My capstone project about Twitter bot detection. You can find the full paper [here](https://ieeexplore.ieee.org/document/10296706) 🎯

I was responsible for creating and testing a random forest model to predict the possibility of a Twitter account being a bot. I made sure the model wasn't overfitting and was learning the data as well as it could.
We gathered around 307k user data and found nearly 15k possible bot accounts in the dataset we gathered. 

I used diffrent datasets variations we created from the actual data we collected. 
(Different size sets with different ratios)

## Datasets
### Mini Datasets
The first mini data set (Data set-1) consists of 5,000
bots and 5,000 normal accounts. The second mini data set
(Data set-2) contains the same number of accounts, but 3,000
of them are bots and 7,000 are normal accounts. Both data
sets consist of the 20 features. In both data
sets, we used a 70%-30% train-test split.

### Large Datasets
We construct two data sets with different bot-normal account
ratios. Data set-3 has 50% bots and 50% normal accounts,
13,581 each in number, in total comprising 27,162 rows.
Data set-4 has 30%-70% ratio of bot and normal accounts,
respectively; this data set contains 13,581 bot accounts and
31,689 normal accounts, summing up to 45,270 rows.

## Results and graphs
- The Random Forest model performs better on a larger data set with 45,270 accounts.
- The model is optimized with hyperparameter values of max depth=10, min samples split=5, n estimators=200, min samples leaf=1.
- The model performs better than other models on both percentages of bot accounts in the data set.
- The accuracy of the model can reach 98% on a data set with 30% bot accounts.

  
![image](https://github.com/acelyasn/capstone/assets/122313795/137275a0-0948-47a4-a34b-327d788f06d3)

![image](https://github.com/acelyasn/capstone/assets/122313795/3f2f5884-168a-4c27-8d79-7aa44732c78e)



Learning curves, ROC curve and confusion matrix can be seen in the code and below:  

- Confusion Matrix of the model:
  Made two different matrix for test and train sets to make sure there was no big difference between two sets

  ![image](https://github.com/acelyasn/capstone/assets/122313795/453537a1-caa0-44ff-800c-28fc32f9a55e)
- Learning Curve of the model:
  Firstly, there isn't a big difference between validation and training, which is an indicator that the model has a good learning process.
  The fact that the training score is slightly decreasing shows that the model is learning and not memorizing patterns.
  
  ![image](https://github.com/acelyasn/capstone/assets/122313795/69805d0f-a5dc-43cb-83b5-5b53e01d3195)

