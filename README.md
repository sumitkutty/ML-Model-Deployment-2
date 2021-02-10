# Streamlit ML Deployment
Machine Learning Model deployment using Streamlit and Heroku
<br />

App Link: https://estream-app.herokuapp.com
## Objective:
#### Predicting the selling price of a car given features like kms driven, transmission type, year bought, present price etc and creating an app using streamlit to following a deployment to heroku.

## Dataset: 
#### The dataset's was collected from cardekho.com.
Link: https://www.kaggle.com/nehalbirla/vehicle-dataset-from-cardekho
* No of features: 9
* No of observations: 301

## Packages:
* Numpy, Pandas, Matplotlib, Flask, Pickle, sklearn

## Preprocessing:
* **Null Values** : There are no null values in the dataset.
* **Feature Elimination**: The 'Car_Name' feature was removed as it would not contribute in a beneficial way. The 'Year' feature was also removed.
* **Feature Engineering**: The 'car_age' feature was computed by calculating the difference between 'Year' variable and current year.
* **Encoding**: The categorical features 'Fuel_Type', 'Seller_Type', 'Transmission' were one-hot encoded.

## Predictive Modelling:
* **ML ALgorithms**: Random Forest was used for the training process.

## Evaluation:
* **Metrics**: R<sup>2</sup>, adjusted  R<sup>2</sup>, negative mean squared error.

## Performance (Random Forest):
* R<sup>2</sup>: 0.9477
* adjusted R<sup>2</sup>: 0.9300
* neg mean squared error:  -2.44


## Productionisation:
### App:
**Streamlit**: Streamlit is a simple appication framework in python. It is gaining some popularity for being a comparatively better option than Flask as the entire app is written in one place and for its feature of writing apps quickly.
Steps:
* Created an app, and wrote a prediction function to predict a car's selling price given the input features.
* The GUI is written in the same python app file under a main function. The GUI is mostly written in HTML/CSS. 
* The GUI contains input spaces for the user to enter values into.
* The prediction function then returns the output to the web page.

### Deployment:
**Heroku**: Heroku is a cloud based PaaS platform. It is used to operate and work on applications directly on the cloud. Heroku was used in this project to deploy the flask app to the web.
Steps:
* Created supported files for heroku.
* Created a process file for heroku execution.
* Pushed the entire app to the git remote repository of heroku.
* The url of the app was created.

# THE END
