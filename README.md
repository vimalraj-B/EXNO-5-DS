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
plt.plot(x1,y1, label="line 1", linewidth=6)
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2, label="line 2", linewidth=6)
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title("Two lines on same graph")
plt.legend()
```
![Screenshot 2025-04-22 112658](https://github.com/user-attachments/assets/acb0019c-1fef-4aa1-993e-fa616bfcd72e)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='blue', linestyle='dashed', linewidth=4, marker='o', markerfacecolor='red', markersize=14)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Some Cool Customizations')
```
![Screenshot 2025-04-22 112759](https://github.com/user-attachments/assets/9e8183cd-1582-42a9-9c6a-6424bbe892b1)

```
years =range(2000, 2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896,]
plt.plot(years, apples, color='red', linewidth=5)
plt.plot(years, oranges, color='orange', linewidth=5)
plt.xlabel('YEAR')
plt.ylabel('Yields (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples', 'Oranges'])
```
![Screenshot 2025-04-22 112847](https://github.com/user-attachments/assets/6e883a7b-9b62-4db2-8ab6-de4a023c7a94)

```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=100,c='red')
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Scatter Plot')
```
![Screenshot 2025-04-22 112922](https://github.com/user-attachments/assets/d3b22cff-de2d-4223-a2e4-3ad0628470de)

```
import matplotlib.pyplot as plt
x_values=[1,2,3,4,5,6,7,8,9,10]
y_values=[2,4,5,7,6,8,9,11,12,12]
plt.scatter(x_values,y_values, label='stars', marker='*',s=300,c='blue')
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Scatter Plot Star')
plt.legend()
plt.savefig("StarScatter.png")
```
![Screenshot 2025-04-22 112953](https://github.com/user-attachments/assets/2ff975c5-ea48-4c0c-8dc1-514a8b74d5b6)

```
import matplotlib.pyplot as plt
x= [1,2,3,4,5,6,7,8,9]
y=[1,4,9,16,25,36,49,64,81]
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Scatter Plot Star')
plt.subplot(2,2,1)
plt.plot(x,y, 'ro--')
plt.subplot(2,2,2)
plt.plot(y,x, 'g*--')
plt.subplot(2,2,3)
plt.plot(x,x, 'bo')
plt.subplot(2,2,4)
plt.plot(y,y, 'go')
```
![Screenshot 2025-04-22 113028](https://github.com/user-attachments/assets/d7b4dd03-4cae-4534-816f-b3386336a576)

```
import numpy as np
np.pi
```
![Screenshot 2025-04-22 113100](https://github.com/user-attachments/assets/b983cbe6-b920-4d7b-8ea3-47de87157f68)

```
X=np.arange(0,4*np.pi,0.1)
Y=np.sin(X)
plt.title("Sin Wave Form")
plt.plot(X,Y, linewidth=5,c='green', linestyle='dotted')
```
![Screenshot 2025-04-22 113126](https://github.com/user-attachments/assets/921252e9-1093-4003-8b27-e820abc1a7aa)

```
import matplotlib.pyplot as plt
import numpy as np
x= [1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between (x,y1, color='red')
plt.fill_between (x,y2, color='blue')
plt.plot(x,y1, color='black')
plt.plot(x,y2, color='white')
plt.legend(['y1','y2'])
plt.show()
```
![Screenshot 2025-04-22 113159](https://github.com/user-attachments/assets/3cb3805e-456b-461c-a823-958067a0a7a7)

```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['One', 'Two', 'Three', 'Four', 'Five']
c1=['g','b']
plt.bar(names, height, width=0.8,color=c1)
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Bar Graph')
```
![Screenshot 2025-04-22 113239](https://github.com/user-attachments/assets/9f3298cf-aa2d-40a7-a4b8-23eb5b36d7ff)

```
x = [2, 8, 10]
y = [11, 16, 9]
x2 = [3, 9, 11]
y2 = [6, 15, 7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='y')
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Bar Graph')
```
![Screenshot 2025-04-22 113320](https://github.com/user-attachments/assets/663e6225-a494-4a6e-b67d-3e3b53c2b73f)

```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90, 77, 32, 21, 20, 40]
range=(0,100)
bins=10
plt.hist (ages, bins, range, color='orange', histtype='bar', rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no.of people')
plt.title('Histogram')
```
![Screenshot 2025-04-22 113400](https://github.com/user-attachments/assets/2591d8f3-91a4-498e-9b66-0ac8dcf7406d)

```
import matplotlib.pyplot as plt
x= [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='grey', alpha=0.5)
plt.show()
```
![Screenshot 2025-04-22 113439](https://github.com/user-attachments/assets/bd498374-b56e-41d9-b80a-e90c05829e8c)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![Screenshot 2025-04-22 113512](https://github.com/user-attachments/assets/1b007f85-6e6f-41f6-9f1e-14214d322de8)

```
fig,ax=plt.subplots()

ax.boxplot(data)

ax.set_xlabel('Data')

ax.set_ylabel('Value')

ax.set_title('Box Plot')
```
![Screenshot 2025-04-22 113539](https://github.com/user-attachments/assets/651b70ed-6814-4acb-a6c6-b17a43af3ec5)

```
import matplotlib.pyplot as plt
activities=['Eat', 'Sleep', 'Work', 'Play']
slices=[3,7,8,6]
colors=['yellow', 'blue', 'orange', 'red']
plt.pie(slices,labels=activities, colors=colors, startangle=90,shadow=True, explode=(0,0.1,0,0), autopct='%1.1f%%')
plt.title('Pie Chart')
plt.show()
```
![Screenshot 2025-04-22 113616](https://github.com/user-attachments/assets/f40ec0fc-705b-4682-bab2-d03391b3f4f7)

```
labels=['Python', 'C++', 'Ruby', 'Java']
sizes=[215,130, 245, 210]
colors=['orange', 'yellow', 'red', 'blue']
explode=(0.1,0,0.1,0)
plt.pie(sizes,explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True, startangle=90)
plt.axis('Equal')
plt.show()
```
![Screenshot 2025-04-22 113641](https://github.com/user-attachments/assets/ea7e15b1-0bd0-43df-818b-6d690e6043b7)


# Result:

```
Thus the program to Perform Data Visualization using matplot python library for the given datas is been implemented.
```
