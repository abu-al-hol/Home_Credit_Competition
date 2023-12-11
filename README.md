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

Implementing the XGBoosted model proved invaluable for enhancing loan approval processes. While the model's technical metrics are impressive, its real business value lies in its ability to inform Home Credit business leaders about potentially risky loan applications and deny such loans from the get-go. By accurately predicting loan defaults, the model is a crucial tool in identifying and avoiding lending to high-risk customers. This capability reduces financial losses from defaults and streamlines the loan approval process, ensuring that the company allocates its resources to creditworthy customers. The insights provided by the model empower business leaders to make data-driven decisions, fostering a more secure and profitable lending environment. This strategic approach to loan issuance solidifies Home Credit's position in the market, emphasizing responsible lending practices and financial prudence. 

## Difficulties 


In tackling the Home Credit dataset, our group encountered various challenges due to the dataset's complexity. The data had many missing values and inconsistencies, requiring extensive cleaning and preprocessing. We spent considerable time handling outliers, filling in missing data, and converting categorical information into a usable format. This process relied on technical skills, problem-solving, and persistence, which are vital when dealing with such gnarly data. Ultimately, from the 120+ variables included in the original data, we used only 49 total variables. The best part about the problems with this exercise was the effort spent understanding, cleaning, and imputing data and watching our metrics and model improve each time we made a smart adjustment. 


## Lessons Learned

The first lesson I took from this is that there is NEVER enough cleaning and EDA to do. Feature engineering is also critical, but this cannot happen until you know your data extremely well.  THis means, if you want to try this competition, you will have to spend hours upon hours really getting to the heart of each variable and knowing what it is and what it does and how it works with other variables.  This seems painstaking and hard, but in reality it is the journey in the data science that makes the results more (or less) fulfilling. I wish I had done a better job of knowing my data. Not until I had completed it, worked in tandem with my team observing their results, did I know what I would have done (or could to) in an iterative fashion to REALLY show these results in the real world. Furthermore, the focus ALWAYS needs to be on business value and showing, even using sample dollars, what employing a model can theoretically do for a company's bottom line. 

## Conclusion

I have to get a plug in here for the R programming language and Posit cloud. I used Posit cloud exclusively and then used R studio desktop to make last minute changes. The amount of computing power required to do an XGBoosted model with the size of data in hand demanded a very powerful Posit cloud virtual machine set up. R is great, it is easy to use, and self contained. Many more people use Python for this work, but in this case R studio and Posit cloud was super easy and reliable. I suggest anyone try to tackle this Kaggle competition, with a team or without, and you will come away much better at ML and predictive models than you were when you started. 

~ All the best,  Jake Jarrard