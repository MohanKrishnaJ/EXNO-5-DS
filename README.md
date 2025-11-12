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
### Simple two lines
```python
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[1,4,1]
plt.plot(x1,y1, label="line 1", color="maroon", linewidth=2)

x2=[1,2,3]
y2=[4,1,4]
plt.plot(x2,y2, label="line 2", color="black", linewidth=2)

plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("Two lines on the same graph")
plt.legend()
```
<img width="739" height="507" alt="image" src="https://github.com/user-attachments/assets/45004ae6-6e39-47f5-8bb7-07bfce84fa3f" />


### Customization of plots
```python
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='grey', linestyle='dashed', linewidth=3, marker='o', markerfacecolor='maroon',markersize=10)

plt.ylim(1,8)
plt.xlim(1,8)

plt.xlabel('x-axis')
plt.ylabel('y-axis')

plt.title("Customization of Plots")
```
<img width="734" height="504" alt="image" src="https://github.com/user-attachments/assets/593b5cb2-1962-4c16-ad9e-cdadae4f664f" />


### Implementation using Matplotlib
```python
yield_orange=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(yield_orange, color='sienna', linewidth=3)
```
<img width="744" height="467" alt="image" src="https://github.com/user-attachments/assets/077df05d-afc8-4b65-b38b-5131d332f7be" />

```python
years= [2010, 2011, 2012, 2013, 2014, 2015]
yield_apples=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(years, yield_apples, color='chocolate', linewidth=3)
```
<img width="649" height="456" alt="image" src="https://github.com/user-attachments/assets/2794ed6f-5a45-4a0d-aae0-da0a89402379" />


```python
years = range(2000, 2012) 
apples = [0.895, 0.91, 0.919, 0.926, 0.929, 0.931, 0.934, 0.936, 0.937, 0.9375, 0.9372, 0.939]
oranges = [0.962, 0.941, 0.930, 0.923, 0.918, 0.908, 0.907, 0.904, 0.901, 0.898, 0.9, 0.896, ] 
 
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)'); 


plt.plot(years, apples)
plt.plot(years, oranges)

plt.xlabel( 'Year')
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in Kanto")
plt.legend(['Apples', 'Oranges'])
```
<img width="747" height="509" alt="image" src="https://github.com/user-attachments/assets/f578991c-df1a-47b4-b131-76f3847cc9cf" />

```python
plt.figure(figsize=(12, 6))
plt.plot(years, oranges, marker='o')
plt.title("vield of Oranges (tons per hectare)") 
```
<img width="1059" height="572" alt="image" src="https://github.com/user-attachments/assets/f83c417c-847b-43a2-b39a-aabb387c19bc" />

```python
plt.plot(years, apples, marker='o')
plt.plot(years, oranges, marker="x")
plt.xlabel('Year') 
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in Kanto")
plt.legend([ 'Apples', 'Oranges']) 
```
<img width="765" height="494" alt="image" src="https://github.com/user-attachments/assets/6447fd6e-2e50-43ff-a1f6-0f723e0334a7" />


### Scatter Plot
```python
import matplotlib.pyplot as plt
x_values = [0,1,2,3,4,5]
y_values = [0,1,4,9,16,25]
plt.scatter(x_values, y_values,s=30, color="blue") 
plt.show() 
```
<img width="765" height="449" alt="image" src="https://github.com/user-attachments/assets/1446b3f3-fa01-49a4-b6b3-440e2dc532c8" />


```python
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
```
![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/3c1770fb-7d88-4ed7-a150-55be14618969)

![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/bef711a9-ddd6-49ff-bb17-26f3d080a123)

```python
plt.scatter(x,y,c="r")
plt.xlabel( 'X axis')
plt.ylabel('Y axis')
plt.title( 'Graph in 2D')
plt.savefig('Test.png')
```
<img width="706" height="487" alt="image" src="https://github.com/user-attachments/assets/decd5b09-81a3-4c1e-804d-9b4ba781da0f" />


![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/7a01f98b-1e1f-47a5-a04e-c0720e308590)

```python
plt.plot(x,y, 'g*',linestyle='dashed' ,linewidth=2, markersize=12)
plt.xlabel( 'X axis') 
plt.ylabel( 'Y axis')
plt.title('2d Diagram') 
```
<img width="682" height="505" alt="image" src="https://github.com/user-attachments/assets/1350898b-b23a-4bc9-974c-d975128dd718" />


![image](https://github.com/varshasharon/EXNO-5-DS/assets/98278161/1d0a16e4-1402-4725-9696-a66465327143)

```python
x = np.arange(0, 4 * np.pi, 0.1) 
y= np.sin(x)
plt.title('sine wave form')
plt.plot(x, y)
plt.show() 
```
<img width="722" height="469" alt="image" src="https://github.com/user-attachments/assets/094b7bb8-2806-4437-b062-c822bf7160bd" />


### Area Chart
```python
import matplotlib.pyplot as pit
import numpy as np
x=[1,2,3,4,5]
y1=[10, 12, 14, 16, 18]
y2=[5,7,9, 11, 13]
y3=[2,4,6,8,10]
pit.fill_between(x, y1, color='maroon')
plt.fill_between(x, y2, color='orange') 
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show() 
```
<img width="622" height="438" alt="image" src="https://github.com/user-attachments/assets/0d3cd464-b70e-497f-9bf9-b9d13eba09cb" />

### Bar Chart
```python
import matplotlib.pyplot as plt

height = [10, 24, 36, 40, 5]
names = ['one','two"', 'three’', 'four', 'five']

c1 =['chocolate', 'darkgreen']
c2 =['skyblue', 'blue'] 
plt.bar(names, height, width=0.8, color=c1)

plt.xlabel('x - axis')

plt.ylabel('y - axis')

plt.title('Bar Chart')

plt.show() 
```
<img width="670" height="492" alt="image" src="https://github.com/user-attachments/assets/8756efa5-826c-425b-adcd-e1fd64d35c52" />


```python
x = [2,8,10]
y = [11,16,9]
x2 = [3,9,11]
y2 = [6,15,7] 
plt.bar(x, y,color='chocolate')
plt.bar(x2, y2, color = 'darkgreen')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show() 
```
<img width="726" height="519" alt="image" src="https://github.com/user-attachments/assets/a9a82e18-8b4e-4aad-bcd1-aa96f52a9934" />

### Histogram
```python
import matplotlib.pyplot as plt

ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range = (0, 100)
bins = 10

plt.hist(ages, bins, range, color='darkgreen' , histtype='bar', rwidth=0.8)

plt.xlabel('age') 

plt.ylabel('No. of people')

plt.title('My histogram')

plt.show() 
```
<img width="704" height="523" alt="image" src="https://github.com/user-attachments/assets/bd7b55ca-17c5-494c-9b93-4da06f4b19af" />


### Box Plot
```python
import matplotlib.pyplot as plt
import numpy as np 

np.random.seed(0) 
data = np.random.normal(loc=0, scale=1, size=100)
data 
```
<img width="690" height="386" alt="image" src="https://github.com/user-attachments/assets/71f99cf2-9c70-4d11-b1c0-da947553fccf" />


```python
fig, ax = plt.subplots() 
ax.boxplot(data) 
ax.set_xlabel('Data') 
ax.set_ylabel('Values')
ax.set_title('Box Plot') 
```
<img width="736" height="500" alt="image" src="https://github.com/user-attachments/assets/66292518-7c23-4e93-b38b-58bcf6d79600" />

### Pie Chart
```python
labels = 'Python', 'C++', 'Ruby', 'Java'
sizes = [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0, 0.4, 0, 0.5)

plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show() 
```
<img width="678" height="434" alt="image" src="https://github.com/user-attachments/assets/df0d7d3e-242f-499f-80a2-efa21da1e777" />


```python
activities = ['eat', 'sleep', 'work', 'play']

slices =[3,7,8,6]

colors=['r', 'y', 'g', 'b']

plt.pie(slices, labels = activities, colors=colors, startangle=90, shadow = True, explode = (0, 0, 0.1, 0), radius = 1.2, autopct = '%1.1F%%')

plt.legend()
```
<img width="595" height="477" alt="image" src="https://github.com/user-attachments/assets/9e8ebbff-8992-4fa3-8213-8a29c3f55466" />


# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.
