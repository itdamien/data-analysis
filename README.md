#import libraries
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error,r2_score
from sklearn.preprocessing import LabelEncoder
#load dataset
data = pd.read_csv('dataset_mid_term.csv')
#display first 5 rows
print(data.head())
#explain each column present
print(data.info())
print(data.describe())
#data cleaning
#checking  missing values
print(data.isnull().sum())
#checking duplicates
print(data.duplicated().sum)
#remove incorrect data
data.dropna()
print(data.dropna())
#data visualization
plt.figure(figsize=(6,4))
sns.heatmap(data.columns(x and y),annot=True)
plt.title("visual title")
plt.show()

plt.figure(figsize=(6,4))
sns.histplot(data[data.columns], bin=20, kde=True)
plt.title(f"distribution of {data.column[o]}")
plt.show()
#scatrer plot of petal length vs petal width
plt.figure(figsize=(6,4))
sns.scatterplot(x = data.columns[0], y = data.columns[1], data=data)
plt.title(f"description of {data.columns[0] and data.columns[1]}")
plt.show()

#heatmap showing correlation among features
sns.heatmap(f"heatmap correlation")

#building model
x = data[num_cols[:-1]]
y  = data[num_cols[:-1]]
x_train, x_test, y_train, y_test(x, y, test_size=0.2, random_state=42)
#build model
model = LinearRegression
model.fit(x_train, y_train)
#model evaLUATION
#predict
y_pred = (x_test)
# evaluate accuracy
mse = mean_squared_error(y_test, y_pred)
r2 = r2_score(y_test, y_pred)
#comment model perfomance
print(f"mean squared error {mse}")
print(f"r-squared error {r2}")
#reflection
print(f" firstly i have learnt how i can debug challenging errors , i have faced full of challenges , data cleaning help our model to be accurate because remove duplicates missing ")






