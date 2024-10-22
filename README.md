# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

## Developed by: G.Keerthana
## Reg.No:212223240045

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import matplotlib.pyplot as plt

x=[1,2,3]
y=[2,4,1]

plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')

plt.title('Two lines on the same graph')

plt.legend()

plt.show()
```
![image](https://github.com/user-attachments/assets/ade639af-0d60-4443-b64e-16235a690975)

```
x1=[1,2,3]
y1=[2,4,1]

plt.plot(x1,y1,label='line 1')

x2=[1,2,3,]
y2=[4,1,3]

plt.plot(x2,y2,label='line 2')

plt.xlabel('x-axis')
plt.ylabel('y axis')

plt.title('Two lines on the same graph!')

plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/0acd62c1-27f3-4bbb-b2ca-df24fd2451c5)

```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]

plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)

plt.ylim(1,8)
plt.xlim(1,8)

plt.xlabel('x-axis')
plt.ylabel('y-axis')

plt.title('Some cool customization')

plt.show()
```
![image](https://github.com/user-attachments/assets/28a4b676-98c9-440e-8403-a9949f44563d)
```
yeild_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yeild_apples)

```
![image](https://github.com/user-attachments/assets/3b565473-4730-459e-8888-80752c48140c)

```
years=[2010,2011,2012,2013,2014,2015]
yeild_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yeild_apples)

```
![image](https://github.com/user-attachments/assets/cf616547-fa4f-4cac-b50e-a30dad37205f)
```
years=range(2000,2012)

apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.962,0.941,0.93,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896]

plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('year')
plt.ylabel('Yield (tons per hectare)')

plt.title('Crop Yeilds in kanto')
plt.legend(['apples','oranges'])
```
![image](https://github.com/user-attachments/assets/e9886cc6-8ec4-4ee2-b6a7-6cee6b485e1b)

```
import matplotlib.pyplot as plt

x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color='blue')
plt.show()
```
![image](https://github.com/user-attachments/assets/55b1f65a-6c64-4be7-ad19-25b840bce574)
```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6,7,8,9,10]
y=[2,4,5,7,6,8,9,11,12,12]

plt.scatter(x,y,label='stars',color='green',marker='*',s=30)

plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title(' My Scatter Plot')
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/3fca1103-a7a6-42c9-9799-82d3016fe30e)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

x=np.arange(0,10)
y=np.arange(11,21)
x
y

```
![image](https://github.com/user-attachments/assets/a79e0a9e-f97e-4e54-b614-bf5dab331565)
```
plt.scatter(x,y,c="r")
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('graph in 2D')
plt.savefig('test.png')

```
![image](https://github.com/user-attachments/assets/7dfdba0d-85be-41ee-806d-6a1bfd71e7b7)
```
y=x*x
y
```
![image](https://github.com/user-attachments/assets/56080162-d303-4b29-a1c2-91b84e641d24)
```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('2D diagram')

```
![image](https://github.com/user-attachments/assets/bbd1097d-d9ce-4423-b62c-a88f857d4d6b)
```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(y,x,'g*')
plt.subplot(2,2,3)
plt.plot(x,x,'bo')
plt.subplot(2,2,4)
plt.plot(y,y,'go')
```

![image](https://github.com/user-attachments/assets/e015c75e-fac3-45b8-9fbc-91fb6a94892a)
```
np.pi
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title('sine wave')
plt.plot(x,y)
plt.show()

```
![image](https://github.com/user-attachments/assets/1b37a2f0-969f-4df4-a8e6-5c48bb8cf932)
```
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
![image](https://github.com/user-attachments/assets/0b01f138-084c-4ebe-b5fa-9c2c1bcee9ce)
```
plt.stackplot(x,y1,y2,y3,labels=['Line 1','Line 2','Line 3'])
plt.legend(loc='upper left')
plt.title(';Satcked Line Chart')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/9ec6eebf-df9b-4fcf-9799-aa54ded40935)
```
from scipy.interpolate import make_interp_spline
x=np.array([1,2,3,4,5,6,7,8,9,10])
y=np.array([2,4,5,7,8,8,9,10,11,12])
spl=make_interp_spline(x,y)


x_smooth=np.linspace(x.min(),x.max(),100)
y_smoooth=spl(x_smooth)
plt.plot(x,y,'o',label='data')
plt.plot(x_smooth,y_smoooth,'-',label='spline')
plt.legend()
plt.show()

```
![image](https://github.com/user-attachments/assets/d1a11a60-bf4f-4d09-bfff-9f449e3045b0)
```
values=[5,6,3,7,2]
names=["A","b","C","D","E"]

plt.bar(names,values,color="green")
plt.show()

```
![image](https://github.com/user-attachments/assets/7f4e2782-22a2-454d-8fcb-9fae1bc6b729)
```
plt.barh(names,values,color="yellowgreen")
plt.show()
```
![image](https://github.com/user-attachments/assets/41502a3e-0732-47a8-8c8e-457f23f8730d)
```
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('-axis')
plt.ylabel('y-axis')
plt.title('My bar chart')
plt.show()

```
![image](https://github.com/user-attachments/assets/2995ffdb-2f2c-49b7-bc28-88ac69eb6774)
```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('bar graph')
plt.xlabel('x-axis')
plt.ylabel('y-axis')

plt.show()
```
![image](https://github.com/user-attachments/assets/347a4d06-ef7e-4bca-9f44-2adc3759f009)
```
ages=[2,5,70,40,30,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('number of people')
plt.title('histogram')
plt.show()
```
![image](https://github.com/user-attachments/assets/8790ace7-c6e5-471a-9e48-05a97e390860)
```
x=[2,1,6,4,2,4,8,9,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]

plt.hist(x,bins=10,color='blue',alpha=0.5)
plt.show()

```
![image](https://github.com/user-attachments/assets/afe76099-b62e-4e83-b59f-116c68c2f83c)
```
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/user-attachments/assets/0bb2ad8e-a24a-4225-a4c1-9dae63bc9ccd)
```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','g','b','y']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0.1,0,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/0b0d9193-ec3d-4ea2-b6ec-b969b359820d)
```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/user-attachments/assets/e4500e33-72b7-4a66-bffa-796acecee690)
```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','g','b','y']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0.1,0,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![image](https://github.com/user-attachments/assets/71fc3040-9cfc-4b01-8e52-562ea0b74c75)

# Result:
Successfully implemented Data Visualization using matplot python library.
