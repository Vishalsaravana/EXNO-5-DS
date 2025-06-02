# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

## Aim:
  To Perform Data Visualization using matplot python library for the given datas.

## EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

## Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

## Coding and Output:


> Developed By: VISHAL S

> REG NO: 212222040181
```py
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

### Line Plot:

```py
marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()

student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()
```

<img src="https://github.com/PSriVarshan/EXNO-5-DS/assets/114944059/cd55b64a-3ec8-49da-89c7-c94ef5eb3dee" width="350" height="350">
<img src="https://github.com/PSriVarshan/EXNO-5-DS/assets/114944059/13bdfe39-d413-48ca-8f73-8719148e5274" width="350" height="350">

### Scatter Plot:

```py
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()

x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```

<img src="https://github.com/PSriVarshan/EXNO-5-DS/assets/114944059/77e6e245-0cd3-4aff-a2e3-e38f06850770" width="350" height="350">
<img src="https://github.com/PSriVarshan/EXNO-5-DS/assets/114944059/f9e6d289-11e7-40d4-9159-edfffb4e5497" width="350" height="350">


### Pie Chart:

```py
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()

feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```


<img src="https://github.com/PSriVarshan/EXNO-5-DS/assets/114944059/d40c68ee-e5db-4674-b3a1-a57a639dfaf9" width="350" height="350">
<img src="https://github.com/PSriVarshan/EXNO-5-DS/assets/114944059/ebb9dd33-8cd3-43d2-8f68-df1c4f9be2d4" width="350" height="350">


### Area Chart:

```py
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```

![image](https://github.com/PSriVarshan/EXNO-5-DS/assets/114944059/423cf3f5-1b02-405c-b11b-770fdb9f58d0)



### Bar Chart:

```py
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```

![image](https://github.com/PSriVarshan/EXNO-5-DS/assets/114944059/19d8b336-1681-4545-b73f-dd72338d9bac)



### Histogram:

```py
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```


![image](https://github.com/PSriVarshan/EXNO-5-DS/assets/114944059/96a8e805-60a8-4ff3-ac33-7e03b5b9bc31)



### Box Plot:

```py
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```


![image](https://github.com/PSriVarshan/EXNO-5-DS/assets/114944059/df37d400-eed0-4c17-a838-d46d0b86200d)


```py
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

![image](https://github.com/PSriVarshan/EXNO-5-DS/assets/114944059/87ce93f0-72b0-4338-a727-7fc0872df45c)


## Result:

### Thus, all the data visualization techniques of matplotlib has been implemented.
