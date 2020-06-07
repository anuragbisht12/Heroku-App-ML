# Build and deploy your first machine learning web app
Components used:
1. jupyter notebook
2. Flask API
3. Model file (pkl)
4. HTML and CSS templates
5. Requirements.txt
6. Proc file


Check the deployed app :https://insuranceregression.herokuapp.com/predict


REST API calls

import requestsurl = 'https://insuranceregression.herokuapp.com/predict'
pred = requests.post(url,json={'age':55, 'sex':'male', 'bmi':59, 'children':1, 'smoker':'male', 'region':'northwest'})
print(pred.json())
