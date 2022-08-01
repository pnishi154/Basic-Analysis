# Basic-Analysis
This is a basic analysis using Jypter notebook


The best place to start in the realm of data science is Jupyter Textbooks. Jupyter provides a workspace that is strong, feature-rich, and easy to use using a variety of installation techniques. Jupyter can be used by users in any setting, regardless of technology.

Big data analysis is significant since it aids in the performance optimization of enterprises. By finding more cost-effective ways to do business and retaining a lot of data, firms can help cut expenses by incorporating it into their business strategy.
#THE PACKAGES WE NEED TO LOAD INTO THE ENVIROMENT INCLUDE
import numpy as np

import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import math 

#WE NEED TO READ THE DATABASE FROM THE SYSTEM IN THE FOLLOWING WAY
#df is my file name
df=pd.read_csv(r'C:/Users/denni/Desktop/survey.csv')
#THE FIGURE SHOWN BELOW SHOWS THE OUTPUT WHEN I LOAD THIS DATABASE INTO MY SYSTEM

![image](https://user-images.githubusercontent.com/49615872/182216538-1383d56a-35e0-49cb-884f-3b39eadaed65.png)


#SOME OTHER BASIC ANALYSIS INCLUDE
#BY USING SEABORN I WAS ABLE TO COME UP WITH VISUALIZATIONS
sns.scatterplot(df['Age'],df['state'], hue =df["family_history"])
![image](https://user-images.githubusercontent.com/49615872/182216906-369e858c-4496-4f6a-bcdd-c737c4bd96fd.png)

#THE DESCRIPTIVE STATISCTIC FOR THIS DATA
![Screenshot (31)](https://user-images.githubusercontent.com/49615872/182218450-f0df3c05-c128-424b-9f7c-04b752728383.png)


#the countplot
sns.countplot(df["Age"])
![image](https://user-images.githubusercontent.com/49615872/182217539-bb3eb7ba-29bc-46b4-9f09-8a527429336c.png)

#the scatter plot
sns.scatterplot(df['Age'],df['state'])
![image](https://user-images.githubusercontent.com/49615872/182217716-a5845a2b-b30d-4648-9bcc-2d31f8ed1a82.png)

#line plot with hue parameters
sns.lineplot(df['Age'],df['Gender'], hue =df["family_history"])
![image](https://user-images.githubusercontent.com/49615872/182217875-43107c58-2236-430b-a338-099754901941.png)

sns.distplot(df['Age'], kde = True, color = "g")
![image](https://user-images.githubusercontent.com/49615872/182218008-137f244d-e165-482f-88a1-b638b47b7624.png)

sns.lineplot( df['Age'], df['Gender'])
![image](https://user-images.githubusercontent.com/49615872/182218158-2e179e53-572c-44ab-8091-caa22b6f9a0c.png)
