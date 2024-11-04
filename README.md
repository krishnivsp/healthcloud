# Healthcloud


During the 2020 global health crisis, there's been a rise in self-diagnosis via online platforms due to readily available information. However, users often misinterpret symptoms and arrive at inaccurate conclusions from medical blogs or notes.

To address these challenges, this project aims to develop HealthCloud, a machine learning-based diagnostic system to monitor the health status of heart patients. We'll assess the accuracy of models like Support Vector Machine, Neural Networks, Logistic Regression, and Gradient Boosting Trees. To enable real-time data analysis, the web interface is deployed on cloud using Render.

Implementations:

Constructed a web interface employing HTML, CSS and JS.
Employed machine learning classification algorithms for monitoring the health status of heart patients.
The best model (i.e. Logistic Regression) was then integrated with the web interface using Flask web framework.
This was later deployed on cloud using Render cloud hosting platform.

Steps to implement this project:

1.Download the dataset 'heart_data.csv'

2.Train the classification models such as LR using the code available in training.py

3.Since the LR model gives the higest accuracy, we will use the trained LR model for futher implementations

4.The trained LR model is stored in 'model.pkl' using 'logistic_regression.py'

5.Create the web interface using 'website.html'(for the home page) and 'predict.html'(for the prediction result page)

6.Integrate the web interface with the trained model using the flask app in 'app.py'

7.'requirements.txt' stores all the dependencies required for this particular project -> pip freeze > requirements.txt

8.'render.yaml'file is a configuration file to define how your application should be built and deployed

9.Go to render cloud platform, create your account, connect your repository containing all the codes and click on deploy
'model.evaluation.py' is an additional comparision of all the classification models on the basis of evaluation metrics

10.Deployed website: https://healthcloud.onrender.com/ (takes about a minute to load since its been deployed using the free tier)
