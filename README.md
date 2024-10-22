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
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/293041a0-f71b-4918-92e7-710a76c3444f)


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

![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/80f9b4fe-48d0-4ca3-82c8-483e8f6233ab)


```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```

![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/28a91459-baef-48e4-8232-75e2824ceb2d)


```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```

![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/12e882d7-747f-4e1c-aab2-8bac0136f13a)


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
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/056a3109-2e4f-4211-8340-cf50baa6b395)


```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```

![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/cfdb20a7-0e0d-43ee-aa74-85edc41f539e)


```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x

```
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/239790ba-c2ed-46df-aed1-f1eefc4017d7)

```
y
```
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/388f936a-f088-446b-8c57-675557764ded)

```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/b98cf287-9d20-4488-aaf6-a1a9f5951ba5)

```
y=x*x
y
```
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/4430d9f4-40fb-447c-b863-ec5b0b98ef7f)

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/8a953236-523a-4a27-9ff4-6fe063766b71)

```
np.pi
```
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/a311a04f-688c-4842-9190-7a379852f20e)

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/c22bfaf9-9ce0-4b64-b82e-0fa07394e8f7)

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
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/1011ec13-d2f9-4e69-9500-cfe7f227a1fc)

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
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/df391761-2480-4f0f-81f7-a0523ccb9c50)

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
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/bbc14531-3a30-41b3-b6b3-321e3a85ca42)

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
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/d7a9e9e9-c6ac-4afb-a9ce-04c53823677f)

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
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/6ea75d19-bacf-46cb-9707-04d8d6c26823)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/25605b60-862f-4cc0-ae37-a690a635d5b5)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/0f1ff5be-4c98-4441-9833-3cb5f763cfb6)


```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/e8a4e3c9-a2fb-469b-b766-add391baff9d)

```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![image](https://github.com/BALUREDDYVELAYUDHAMGOWTHAM/EXNO-5-DS/assets/119559905/8e7b0944-d2fe-4b09-a6e6-e0904ac308d8)

# Result:
  Thus, The implementation of data visualization using matplotlib has been successfully verified.
