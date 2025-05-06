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
 import pandas as pd
 import numpy as np
 import seaborn as sns
 import matplotlib.pyplot as plt
 x = [1, 2, 3, 4, 5]
 y = [3, 6, 2, 7, 1]
 plt.plot(x,y,label='line1')
```
![image](https://github.com/user-attachments/assets/ad9e02a0-6c0e-4943-95b0-566786db9f8f)

```
 x1 = [1,2,3]
 y1 = [2,4,1]
 x2 = [1,2,3]
 y2 = [4,1,3]
 plt.plot(x1,y1,label='line1')
 plt.plot(x2,y2,label='line2')
 plt.xlabel('x-axis')
 plt.ylabel('y-axis')
 plt.title('Two lines on same graph!')
 plt.legend()
 plt.show()
```
![image](https://github.com/user-attachments/assets/1f0f6b98-8f62-432e-b3a4-2c733eff856e)

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
![image](https://github.com/user-attachments/assets/99d60005-ee7c-4b72-add2-ef8276b1b038)

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![image](https://github.com/user-attachments/assets/f8199d4b-1a93-4954-a994-d298ecd66f2c)

```
 years=[2010,2011,2012,2013,2014,2015]
 yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
 plt.plot(years,yield_apples)
```
![image](https://github.com/user-attachments/assets/f168e859-f735-44d2-8dd6-92ef269123d4)

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
![image](https://github.com/user-attachments/assets/deb6c657-815c-4049-a3a6-be6a31dbe6d6)

```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```
![image](https://github.com/user-attachments/assets/4b861384-d2a9-48e6-b0ee-fbe82f00a4a5)

```
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 x=np.arange(0,10)
 y=np.arange(11,21)
 x
```
![image](https://github.com/user-attachments/assets/1588f63a-9376-4393-a141-c9394223209b)

```
y
```
![image](https://github.com/user-attachments/assets/9e5474d5-5337-40fc-83f0-21dba98c34cc)

```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/user-attachments/assets/4ad16a4e-a9bb-429d-976d-13be25ae97b5)

```
y=x*x
 y
```
![image](https://github.com/user-attachments/assets/efbf2914-037c-439c-a211-4b1df7666ffa)

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.legend(['y-values']);
```
![image](https://github.com/user-attachments/assets/ec9ff3d8-7556-4ea0-afc0-d91af57a041f)

```
 x=np.arange(0,4*np.pi,0.1)
 y=np.sin(x)
 plt.title("sine wave form")
 plt.plot(x,y)
 plt.show()
```
![image](https://github.com/user-attachments/assets/e9443937-b285-4fd2-9ac0-f10a05a1c6a8)

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
![image](https://github.com/user-attachments/assets/289654e4-aaf1-4484-95b2-41c351b0fe07)

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
![image](https://github.com/user-attachments/assets/d170865f-1453-470d-bd3e-14f75307711c)

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
![image](https://github.com/user-attachments/assets/8d8f84ab-a50a-4701-a646-3a65cffefaee)

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
![image](https://github.com/user-attachments/assets/35477e9d-822b-4297-8e86-29b76ed9e568)

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
![image](https://github.com/user-attachments/assets/24b057b7-5e0f-4a2e-8d1c-5bf791b88a47)

```
 import matplotlib.pyplot as plt
 import numpy as np
 np.random.seed(0)
 data=np.random.normal(loc=0,scale=1,size=100)
 data
```
![image](https://github.com/user-attachments/assets/8c291f10-90d7-47c7-8964-119a62a4a5fd)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![image](https://github.com/user-attachments/assets/8bfa6804-341e-43f7-9583-85cc9a023544)

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/user-attachments/assets/f6b7b78a-6bce-4fae-b561-cde9e371f7dc)

```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![image](https://github.com/user-attachments/assets/31bcc53d-4e66-482c-a577-aacdded08d02)

# Result:
 Include your result here
