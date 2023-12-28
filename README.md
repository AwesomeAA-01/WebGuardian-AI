# Phishing URL Detection 
![image](https://github.com/AwesomeAA-01/WebGuardian-AI/blob/main/img-1.png)
![image](https://github.com/AwesomeAA-01/WebGuardian-AI/blob/main/img-2.png)
![image](https://github.com/AwesomeAA-01/WebGuardian-AI/blob/main/img-3.png)

## Table of Content
  * [Introduction](#introduction)
  * [Installation](#installation)
  * [Directory Tree](#directory-tree)
  * [Result](#result)
  * [Conclusion](#conclusion)


## Introduction

The Internet has become integral to our lives, yet it also facilitates malicious activities like Phishing. Phishers exploit anonymity to deceive victims through social engineering or mockup websites, stealing sensitive information. Despite evolving detection methods, Machine Learning emerges as a potent tool. Phishing attacks exhibit common characteristics discernible by ML, offering an effective means to counter these threats. 


## Installation
The Code is written in Python 3.11.7. If you don't have Python installed you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory after [cloning](https://www.howtogeek.com/451360/how-to-clone-a-github-repository/) the repository:
```bash
pip install -r requirements.txt
```

## Directory Tree 
```
├── pickle
│   ├── model.pkl
├── static
│   ├── styles.css
├── templates
│   ├── index.html
├── Phishing URL Detection.ipynb
├── Procfile
├── README.md
├── app.py
├── feature.py
├── phishing.csv
├── requirements.txt


```

## Technologies Used

![](https://forthebadge.com/images/badges/made-with-python.svg)

[<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/3/31/NumPy_logo_2020.svg" width=200>](https://numpy.org/doc/) [<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/e/ed/Pandas_logo.svg" width=200>](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html)
[<img target="_blank" src="https://upload.wikimedia.org/wikipedia/commons/8/84/Matplotlib_icon.svg" width=100>](https://matplotlib.org/)
[<img target="_blank" src="https://scikit-learn.org/stable/_static/scikit-learn-logo-small.png" width=200>](https://scikit-learn.org/stable/) 
[<img target="_blank" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcScq-xocLctL07Jy0tpR_p9w0Q42_rK1aAkNfW6sm3ucjFKWML39aaJPgdhadyCnEiK7vw&usqp=CAU" width=200>](https://flask.palletsprojects.com/en/2.0.x/) 

## Result

Accuracy of various model used for URL detection
<br>

<br>

||ML Model|	Accuracy|  	f1_score|	Recall|	Precision|
|---|---|---|---|---|---|
0|	Gradient Boosting Classifier|	0.974|	0.977|	0.994|	0.986|
1|	CatBoost Classifier|	        0.972|	0.975|	0.994|	0.989|
2|	XGBoost Classifier| 	        0.969|	0.973|	0.993|	0.984|
3|	Multi-layer Perceptron|	        0.969|	0.973|	0.995|	0.981|
4|	Random Forest|	                0.967|	0.971|	0.993|	0.990|
5|	Support Vector Machine|	        0.964|	0.968|	0.980|	0.965|
6|	Decision Tree|      	        0.960|	0.964|	0.991|	0.993|
7|	K-Nearest Neighbors|        	0.956|	0.961|	0.991|	0.989|
8|	Logistic Regression|        	0.934|	0.941|	0.943|	0.927|
9|	Naive Bayes Classifier|     	0.605|	0.454|	0.292|	0.997|

Feature importance for Phishing URL Detection 
<br><br>
![image](https://github.com/AwesomeAA-01/WebGuardian-AI/blob/main/img-4.png)




## Conclusion
1.The project's primary objective was to explore a range of machine learning models and conduct in-depth Exploratory Data Analysis on a phishing dataset to gain insights into their distinctive features.

2.The creation of the project notebook proved instrumental in enhancing the understanding of the key features influencing models in determining the safety of URLs, shedding light on the nuanced aspects of model performance and fine-tuning.

3.Notable features such as "HTTPS," "AnchorURL," and "WebsiteTraffic" emerged as crucial factors in differentiating between phishing and non-phishing URLs, underscoring their significance in the classification process.

4.The analysis revealed that the Gradient Boosting Classifier exhibited a remarkable accuracy of 97.4%, showcasing its proficiency in accurately classifying URLs and, consequently, reducing the risk associated with malicious attachments.

5.The conclusive findings emphasized the importance of specific features in the phishing dataset, providing valuable insights for future endeavors in developing and refining machine learning models for URL classification and security.
