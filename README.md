# Home_Credit_Competition
About: My collegiate attempt at the Home Credit Kaggle Competition...

## Introduction

I am currently a candidate for the Master of Science in Business Analytics (MSBA) within the Eccles School of Business at the University of Utah. If you are a college graduate in need of a boost to your career or want to "exponentiate" your data acumen and business background, it's the place to be. Click for more information...

- [University of Utah MSBA Program](https://eccles.utah.edu/programs/master-of-science-in-business-analytics/)

As part of our graduation requirements, MSBA candidates conduct a final capstone project to be presented at the end of the fourth semester where a local (Salt Lake City, Utah) company asks students to use newly acquired machine learning & data science skills to solve a unique data-driven business problem. In preparation for the final capstone, in the third semester, MSBA candidates have to wrestle with and tackle the "Home Credit" Kaggle competition. Needless to say, its a beast of a project. Specific details, to include a download of the data used in this exercise, can be accessed from the competition itself: 

- [KAGGLE: Home Credit Default Risk](https://www.kaggle.com/competitions/home-credit-default-risk)

The data that I used in the above R-Markdown files can be taken from the Kaggle website and you are able to see how I conducted EDA, Data Cleaning & Feature Engineering, and then employed an Extreme Gradient Boosted (XGBoost) algorithm to make predictions about those who would default on loans provided by Home Credit. 

## HTML ouput of R Markdown Documents

I included the following html output pages (knitted R markdown files) that correspond to the original .RMD source files here in this repository. You may view the final HTML output simply by clicking on the following links:

- [Exploratory Data Analysis (EDA)](https://abu-al-hol.github.io/Home_Credit_Competition/EDA.html)
- [Data Cleaning and Feature Engineering](https://abu-al-hol.github.io/Home_Credit_Competition/cleaning-and-engineering.html)
- [Modeling with XGBoost](https://abu-al-hol.github.io/Home_Credit_Competition/Jakes-XGBOOST.html)

A note about usage and licensing. The data belongs to Home Credit and provided by Kaggle. The code above was generate by me with some help from classes, books, previous work and ChatGPT. This was my second attempt at a Kaggle competition.  Fair warning: this is my best attempt, after hours of wrestling and feeling overwhelmed, to create predictions on the Kaggle provided test set for submission; I do not claim that it is the best, but I am proud of it. You may use, abuse and download my R Markdown documents as much as you like, with proper attribution as is proper. However, the learning curve with this was steep and long, and I recommend that if you are a student and aspiring data scientist that you tackle the assignment with the skills you have and avoid drawing on the work of others. The lessons learned after completing the competition were profound. Do not miss this critical learning by using my work as your submission...there's no point in doing so. 

## Business Problem

Home Credit is tackling financial disparities in emerging markets using advanced data analytics to evaluate and predict client credit risk. By integrating historical and real-time data and market-specific insights, the project seeks to refine client risk assessment, thereby reducing the loan default rate from roughly 8% to near zero. This initiative involves analyzing a comprehensive dataset of 356,255 clients to pinpoint key indicators of default risk. The goal is to enhance loan processing efficiency, support responsible lending, and strengthen Home Credit's position in the emerging market sector, ultimately fostering financial inclusion through data-driven decision-making. Home credit called on the skills of data scientists to provide a solution using ML algorithms to predict default moving forward. 

## Solution to the Business Problem


In my work for Home Credit, I faced a skewed target variable with most cases showing no defaults. To deal with this, I adjusted the model to give more weight to the less common default cases. My process started with exploratory data analysis and feature engineering, and finally I relied on two XGBoost models over logistical regression to make predictions. This approach, especially focusing on the minority class, helped me reach an AUC of 0.7859561 and a balanced accuracy of 0.7096. These steps were key to making the model more accurate in predicting loan defaults. My personal goal was to err on the side of capturing as many true positives (people predicted to default, who indeed defaulted) as possible. I applied this predictive model to the test set, which ultimately landed me a Kaggle score of .7338.   

## My Contribution

The work you see included here is my own. However, when our team assembled, our objective was to take the best processes of each member and submit a final Kaggle score correlated to the best AUC as a group. We still utilized an XGBoost model; however, we ran it more than 2000 times to minimize log loss and improve accuracy. Our team also conducted more thorough feature engineering and drew on elements of the ancillary data sets.    

## The Business Value



## Difficulties 


## Lessons Learned

## Conclusion