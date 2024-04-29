# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
 ```
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```
![ds1](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/2b14c461-065e-4265-a225-1453dca5dfe6)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
```
![ds2](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/4343088b-0c73-48f2-98c4-88f4c2b9b6c2)

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![ds3](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/e696808e-1033-4e98-b074-79d6465c1700)

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```
![ds4](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/ca8de539-2cbf-446f-8615-b258ed9f5286)

```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);
```
![ds5](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/2ca7ac58-bd47-49d2-b720-f983caaa97e8)

```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```
![ds6](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/c95d192b-1cd4-4b65-ba92-726f9d818ec2)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```
![ds7](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/ec728ecb-0d0d-4ba6-820f-cefcaf83cc1a)

```
y
```
![ds8](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/a80c7d2b-e9c6-4584-89db-1fa04675249f)

```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![ds9](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/64ae465b-72c6-409a-89e5-bfce6dc7cf81)

```
y=x*x
y
```
![ds10](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/a12ea954-4c6d-43f3-9e54-429fde7a5f7a)

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```
![ds11](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/f31df484-1486-4368-a3c7-9266d2cafc33)

```
np.pi
```
![ds12](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/fb997f6e-b27a-4592-94e9-cbcefb2aaf16)

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
![ds13](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/5b82ee82-2781-434e-99d4-586ceafc6312)

```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
```
![ds14](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/476b8ba6-ab1d-4d99-87f0-c2508f5e22d2)

```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')

plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
![ds15](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/26244687-c8b1-4a0b-997e-fd1ad29fd9a1)

```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```
![ds16](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/2483a6e3-ef94-4b42-a786-015ad1ab2753)

```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![ds17](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/5f37400b-2c87-4c31-9336-2a71f93ca592)

```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```
![ds18](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/a29cc865-1459-47ac-9004-1dff6112d282)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![ds19](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/ad8121df-c98e-4332-b469-56e312d873de)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![ds20](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/fd7e2f18-9531-4add-b40a-633be307e2b3)

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![ds21](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/a84a7923-ba7e-4292-9a74-3e2e3a829f4b)

```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![ds22](https://github.com/DHINESH-SEC/EXNO-5-DS/assets/119560302/d579c50b-5497-4e00-90d8-c56b5cc88e0b)

# Result:
  Thus, The implementation of data visualization using matplotlib has been successfully verified.
