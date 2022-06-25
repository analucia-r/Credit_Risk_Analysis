# Credit_Risk_Analysis

## Overview of the analysis: 
Credit risk is usually very tough to predict but while using Machine Learning  we can leverage large datasets and determine patterns to construct useful recomendations. 
Machine learning adds analytical value and has the potencial to uncover subtle relationships. During this project we took in consideration the factors in our csv files about loan statstistics and help predict if someone is on high or low risk. The specific libraries we are using are imbalanced-learn and scikit-learn, it is important to install these libraries under the machile leanring enviroment because if you are using jupyter by defult it will upload in the Python enviroment. With these libraries, we built models to evaluate different methods by oversampling/undersampling the data using smote algorithms and clustercentroid.  


## Results 
### RandomOver Sample model 
<img width="600" alt="1" src="https://user-images.githubusercontent.com/92067596/175787323-b9b37ad5-6a15-444a-b726-956c58da1fc9.png">

<img width="600" alt="3" src="https://user-images.githubusercontent.com/92067596/175787390-72354df6-9f99-4de0-acdf-ab2b039ca4d4.png">
Balance accuracy score is 65%, Due to the high number of the low_risk population it's precisions is almost 100% witha  sensitivity of 66%.  


### SMOTE model
<img width="800" alt="image" src="https://user-images.githubusercontent.com/92067596/175787512-31bac145-8656-4d5b-8ca5-4ad45d23de11.png">

Balance accuracy score is 65%, Due to the high number of the low_risk population it's precisions is almost 100% witha  sensitivity of 66%.  

### ClusterCentroids model
<img width="800" alt="image" src="https://user-images.githubusercontent.com/92067596/175787548-3ecb94e0-2f9b-4418-af5d-1005e5e812d8.png">
Balance accuracy score is 52%, due to high number of false positives shows the rec is a low_risk sensitivity at 40% 

### SMOTEEN MODEL 
<img width="800" alt="image" src="https://user-images.githubusercontent.com/92067596/175787605-6f702de1-d8a4-4315-a0b1-a8ba36deb7f4.png">
Balance accuracy score is 62%, high number of false positives, the low_risk sensitivity is 57%.

### BalancedRandomForestClassifier model
<img width="800" alt="image" src="https://user-images.githubusercontent.com/92067596/175787707-af3f3984-be35-436e-8997-4140fb96e955.png">
Balance accuracy score is 79%, lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.

### EasyEnsembleClassifier model
<img width="800" alt="image" src="https://user-images.githubusercontent.com/92067596/175787750-d8342573-0d32-4b84-a7cf-637152de5610.png">
Balance accuracy score is 93%, ower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.

## Summary  
Typically, in the models you want a good balance of recall and precision which is why the ensemble classifiers is recommended over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. 
