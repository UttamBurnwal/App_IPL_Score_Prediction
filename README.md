# App_IPL_Score_Prediction

--> A Machine Learning Web App that can predict the first inning score of an IPL match. Users provide various inputs such as name of batting team, bowling team, venue and so on. Based on these inputes the app provides a range of scores that the batting team can score. The app is created with the help of ```Flask``` and is currently deployed on ```Heroku``` platform.

Visit: https://ipl-score-app.herokuapp.com/

## A glimpse of the web app


  ![GIF](static/gif.gif)

## Directory Tree
--> Here are some details of the subdirectories and files that the repository contains. 
```
├── static 
│   ├── Images
│   ├── ipl-favicon.ico
│   ├── style.css 
├── template
│   ├── index.html
│   ├── result.html
├── IPL_Prediction_Score.ipynb
├── Procfile
├── README.md
├── app.py
├── ipl.csv
├── ipl_score_model.pkl
├── requirements.txt
```
## Description
* Static Folder contains the images, favicon as well as the css file which depicts the HTML elements of the web app.
* Template folder contains two html file. Index.html file represents the input page where user provides all the input to the web app, while the result.html represents the result part of web page where the user will recieve the predicted score.
* IPL_Prediction_Score.ipynb is a notebook document created by Jupyter Notebook that contains all the notebook code and the execution results that has helped in generating the model for the web app.
* Procfile includes the code ``` web: gunicorn app:app ``` which depicts that gunicorn commands are run by the application's containers on the platform. To create a procfile run the following command on command prompt. ``` echo web: gunicorn app:app > Procfile ```
* README.md includes the stucture that provides a detailed description of my GitHub project.
* app.py includes the all the routes and functions to perform the actions of web app. This file is the root of the Flask application which we will run in the command line prompt.
* ipl.csv is the dataset file which is in the csv format.
* ipl_score_model.pkl is the decision tree regression model which acts as the core of the web application.
* Requirements.txt file includes all the libraries that has been used to create the web app. After installing all the required packages, ``` pip freeze > requirements.txt ``` command was run on the command prompt to create the requirements.txt file

## Libraries Used
--> This section contains the list of the libraries that have been used to create the web app. 
```
certifi==2020.6.20
click==8.0.3
colorama==0.4.4
Flask==2.0.3
itsdangerous==2.0.1
Jinja2==3.0.3
joblib==1.1.0
MarkupSafe==2.0.1
numpy==1.22.2
scikit-learn==1.0.2
scipy==1.8.0
sklearn==0.0
threadpoolctl==3.1.0
Werkzeug==2.0.3
wincertstore==0.2
gunicorn
```



