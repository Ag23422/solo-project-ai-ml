# solo-project-ai-ml

import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
import geo.py as gps
API_KEY = "AkvYaDkG40h_rbg-DIGhsap7cxZic5v4GUlAWqeAMkZ1prAuXXx_TLRUGCrb-Uiv"  # Replace with your Bing Maps API key

geolocator = geopy.geocoders.Bing(AkvYaDkG40h_rbg-DIGhsap7cxZic5v4GUlAWqeAMkZ1prAuXXx_TLRUGCrb-Uiv)



dataset = pd.read_csv('realtor-data.zip.csv')
dataset2= pd.read_csv('test.csv')



a = input("what is your monthley income ")
b= input ("type of property required (enter the no of beds required)")
c=12*int(a)
print(c)
X= dataset.iloc[:, 1:].values
y = dataset.iloc[:, 3].values
z=dataset.iloc[:,1].values


for c in dataset.iloc[:,1].values:
  if(c<=z.all()):
    from sklearn.cluster import KMeans
    wcss = []
    for i in range(1, 11):
      kmeans = KMeans(n_clusters = i, init = 'k-means++', random_state = 42)
    kmeans.fit(X)
    wcss.append(kmeans.inertia_)
  if (int(b)==y.all()):
       from sklearn.cluster import KMeans
       wcss = []
       for i in range(1, 11):
        kmeans = KMeans(n_clusters = i, init = 'k-means++', random_state = 42)
        kmeans.fit(X)
        wcss.append(kmeans.inertia_)

d=input('enter the preffered propetry amount: ')
e=input('enter your gender: ')
g=input('enter your no of dependents : ')
f=input('no of working indivisuals : ')
h=input('total household income : ')
k=input('the loan amount required: ')
i={e,g,f,h,k}

j=dataset2.iloc[:, 11]
o = dataset2.iloc[:, :-1].values
p = dataset2.iloc[:, -1].values

q=input('tenure of loan amount(no of years) : ')
r=

for d in dataset.iloc[:, 1] 
  if (j==1):
    from sklearn.linear_model import LogisticRegression
    classifier = LogisticRegression(random_state = 0)
    classifier.fit(o,p)
    print('your per month payment is : ')
  elif():
    print('you are not eligeble: ')
  
  print(o,p)




