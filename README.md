# project-2-part-4
## prediction of charges
#### buisness problem
This project predicts how additional charges will be based on the data of the patient.
### data source
the learning platform
### Introduction of the Data
Our data is composed of  age, sex, BMI, number of children, smoking habit, region of the patient and charges columns.
Our data has 1337 rows and  it has 7 columns.
Our target valuable will be 'charges' column while the rest of the columns will be features of the data.
### analytical insites from the data
![image](https://github.com/elleniayele/project-2-part-4/assets/61632568/a1d36838-6f35-430f-b324-be79ce261567)
this data shows us that as age increases, so does the charges asked to a patient. which makes sense in a way that as people get older, they are more riskier than the younger patients so the cost is less for younger generation than older generation.
![image](https://github.com/elleniayele/project-2-part-4/assets/61632568/8c2cec35-9fd0-43db-bd56-091a99a245df)
this shows that as child number increases, so does the charges.
### modeling
since the target is the 'charges' column, it is a regression problem. After training and testing our data set and applied preprocessing steps,  i used three kinds of modeling: linear regression,decision tree regression and random forest regression. after processing the data and finding best parameters for the models, the best model i found which is a random forest model with pca applied, here are the results of the metrics:
      
      ### random forest regressiion 
      
        #### r2 score
        
      -Training R2 is 0.9712278015286793
      -Testing R2 is 0.8628933212895309

       #### mean absolute error
       
       - train_MAE:1130.305272327645
       - test_MAE:2846.7845994677605
       
       #### root mean squared error

       - train_RMSE:1989.6214016701506
       - test_RMSE:4868.992751402017
       
 In here, we can say that our model was off on predictions by $ 1130 in the training set and it was off on predictions by $2846.78. That means that since the median price for charges is $9386.16, it was off on it's predictions by about 0.12% on average. and our model is correctly predicting 88% which is preety good.
our model was also accurate on training data by 97% while 86% on the testing data. 

       ### recommendations

      
The data is over fit slightly since it is making  almost good predictions based on what it was trained on but the larger number of errors on testing data. I assume is the is due to the Datas not related to each other that much including the target , I would suggest getting more data from the patients other than five factors so gathering of more data other than 5 columns, so that the model performs better,has more information to be trained on.
second recommendation is that the columns that should be on the data should be more related to the charges column, like patient's health information and other factors that affect patients health.

                                  ### 




  -


  





