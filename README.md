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
![ds1](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/d927ea5d-c3c2-4532-a07f-c6e75604d210)

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
![ds2](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/e78a0f64-68c6-4664-9a88-b220c1edf707)

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![ds3](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/f7874d8f-fe0a-44fa-8ecd-60df0fa3c463)

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```
![ds4](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/3872c2fa-e96a-47b2-99b7-771065989cb7)

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
![ds5](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/a115416f-9fcf-4d99-a4e9-fe3bbd564556)

```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```
![ds6](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/b2e9de64-2f69-4668-9340-4c6fd50dc664)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```
![ds7](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/66693670-eb87-46f1-af91-b4469562502d)

```
y
```
![ds8](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/f0d92978-24f0-42d5-9ff6-db1b24fe915c)

```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![ds9](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/33a4f290-e270-4d1e-a066-4f1901de2f71)

```
y=x*x
y
```
![ds10](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/33ceb57d-3637-419a-8b35-662988040a06)

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```
![ds11](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/8ea9e6ad-19ef-45b0-aed6-3ade2538e6e3)

```
np.pi
```
![ds12](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/f76db70f-5112-48cf-b27e-e776fcf75338)

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
![ds13](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/11159d24-a8fa-427c-9583-3be2629e58c9)

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
![ds14](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/db869d4a-1d32-4082-a8f8-f67b30db3dc2)

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
![ds15](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/caf37c54-2559-4e1b-851d-d503bb6caf5a)

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
![ds16](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/f8f9badf-58a7-428f-b23c-88b1c0d138cd)

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
![ds17](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/1aa70cba-9f22-4d95-b416-1fd817b10f99)

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
![ds18](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/5b3bea86-f4f2-4c99-aff5-2ce4c70d941e)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![ds19](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/df2308c3-9a00-466e-8730-1fbda7c54464)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![ds20](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/ed98d4c8-c211-4629-8c59-a068fcb8b5f4)

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![ds21](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/719a6ced-2215-4ee3-94e4-7597ed963ab2)

```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![ds22](https://github.com/gokulapriya632202/EXNO-5-DS/assets/119560302/78b6950a-1e4b-4c69-a2b0-2f92b11bc78e)

# Result:
  Thus, The implementation of data visualization using matplotlib has been successfully verified.
