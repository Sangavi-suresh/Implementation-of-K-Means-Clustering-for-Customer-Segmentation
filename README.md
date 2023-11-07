# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm:

1. Import dataset and print head,info of the dataset.

2.check for null values.

3.Import kmeans and fit it to the dataset.

4.Plot the graph using elbow method.

5.Print the predicted array.

6.Plot the customer segments.
   
## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: Sangavi Suresh
RegisterNumber:  212222230130
import matplotlib.pyplot as plt

data=pd.read_csv("/content/Mall_Customers (1).csv")

data.head()

data.info()

data.isnull().sum()

from sklearn.cluster import KMeans

wcss=[]

for i in range(1,11):

kmeans=KMeans(n_clusters=i,init="k-means++")

kmeans.fit(data.iloc[:,3:])

wcss.append(kmeans.inertia_)

plt.plot(range(1,11),wcss)

plt.xlabel("No_of_Clusters")

plt.ylabel("wcss")

plt.title("Elbow Method")

km=KMeans(n_clusters=5)

km.fit(data.iloc[:,3:])

y_pred=km.predict(data.iloc[:,3:])

y_pred

data["cluster"]=y_pred

df0=data[data["cluster"]==0]

df1=data[data["cluster"]==1]

df2=data[data["cluster"]==2]

df3=data[data["cluster"]==3]

df4=data[data["cluster"]==4]

plt.scatter(df0["Annual Income (k$)"],df0["Spending Score (1-100)"],c="red",label="cluster0")

plt.scatter(df1["Annual Income (k$)"],df1["Spending Score (1-100)"],c="black",label="cluster1")

plt.scatter(df2["Annual Income (k$)"],df2["Spending Score (1-100)"],c="blue",label="cluster2")

plt.scatter(df3["Annual Income (k$)"],df3["Spending Score (1-100)"],c="green",label="cluster3")

plt.scatter(df4["Annual Income (k$)"],df4["Spending Score (1-100)"],c="magenta",label="cluster4")

plt.legend()

plt.title("Customer Segment")
*/

```

## Output:
# DATA.HEAD():
![image](https://github.com/Sangavi-suresh/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/118541861/67469cc5-c372-4eae-8e16-f7e1c6e1a74c)

# DATA.INFO():
![image](https://github.com/Sangavi-suresh/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/118541861/3909f80e-8eb7-4aa1-9a95-5408285521d3)

# DATA.ISNULL().SUM():
![image](https://github.com/Sangavi-suresh/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/118541861/1941634a-8f66-47d8-a427-dc8f134c8452)

# PLOT USING ELBOW METHOD:
![image](https://github.com/Sangavi-suresh/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/118541861/6be8c005-fe59-4955-a34a-656caaf4142a)

# K-MEANS CLUSTERING:
![image](https://github.com/Sangavi-suresh/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/118541861/eb229033-7212-4c29-a402-a35207fa4cba)

# Y_PRED ARRAY:
![image](https://github.com/Sangavi-suresh/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/118541861/267a4c13-5cbb-4e37-8cfe-b2e703c12907)

# CUSTOMER SEGMENT:
![image](https://github.com/Sangavi-suresh/Implementation-of-K-Means-Clustering-for-Customer-Segmentation/assets/118541861/d3f74e2f-ce3d-4db9-8ec5-76773df8559c)


## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
