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
Developed By: Ashqar Ahamed S.T
Register No.: 212224240018
```
**Line Plot**
```
import matplotlib.pyplot as plt

x_values = [1,4,5,8,13,15,19,22,28]
y_values = [2,4,7,5,8,14,17,20,24]

plt.plot(x_values,y_values)
plt.title("Graph")
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.show()
```

<img width="763" height="768" alt="LP1" src="https://github.com/user-attachments/assets/1851754a-bc9a-4b93-82b6-b1ca5004a8e0" />

```
x_values = [1,4,5,8,13,15,19,22,28]
y_values = [2,4,7,5,8,14,17,20,24]

x2_values = [10,12,14,16,18,20,22,24,26,28,30]
y2_values = [10,11,12,13,14,15,16,17,18,19,20]
plt.plot(x_values,y_values, label="First Line")
plt.plot(x2_values,y2_values, label="Second Line")
plt.legend()

plt.title("Graph of two lines")
plt.xlabel("x-axis")
plt.ylabel("y-axis")
plt.show()
```

<img width="666" height="816" alt="LP2" src="https://github.com/user-attachments/assets/616bbeb2-aecc-42da-b3db-e336affdf9d2" />

```
x = [1,2,3,4,5,6,7,8,9,10]
y = [15,10,15,10,15,10,15,10,15,10]
plt.plot(x,y, color="red", linestyle="dashed", linewidth=3,marker='o',markerfacecolor='yellow', markersize=6)
plt.xlim(0,20)
plt.ylim(0,20)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('customization')
plt.show()
```

<img width="899" height="693" alt="LP3" src="https://github.com/user-attachments/assets/4314dfc4-9c72-433c-90ac-16a4a1af82d8" />

<br>

**Bar Chart**
<br>

```
values =[15,27,38,20,16]
names = ['A','B','C','D','E']

plt.bar(names,values,color='blue')
plt.show()
```

<img width="625" height="542" alt="BC" src="https://github.com/user-attachments/assets/2bbbd511-0825-4ebe-b3c3-18e723471e47" />

<br>

**Scatter Plot**
<br>
```
x_values = [1,4,5,8,13,15,19,22,28]
y_values = [2,4,7,5,8,14,17,20,24]

plt.scatter(x_values,y_values,color='lightgreen',s=20)
plt.show()
```

<img width="658" height="542" alt="SP" src="https://github.com/user-attachments/assets/655836b9-6d06-4881-9400-58a0b9080a72" />

<br>

**Pie Chart**
<br>
```
work = ['college','module','lab','study','record','script','research','edit']
slices = [6,2,1,4,3,2,2,4]

colors = ['r','g','b','c','m','y','purple','lime']
plt.pie(slices, labels=work, colors=colors,startangle=90,explode=(0,0,0,0,0.1,0,0,0),autopct='%1.1f%%')
plt.title('pie chart')

plt.show()
```

<img width="874" height="590" alt="Pie" src="https://github.com/user-attachments/assets/25c7f13d-d719-4fb7-9fe2-db51d7d19c57" />

<br>

**Area Chart**
<br>
```
x = [1,2,3,4,5]
y1 = [10,12,14,16,18]
y2 = [5,7,9,11,13]

plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='red')
plt.plot(x,y1,color='black',label='y1')
plt.plot(x,y2,color='black',label='y2')
plt.legend(['y1','y2'])
plt.show()
```

<img width="769" height="640" alt="Area" src="https://github.com/user-attachments/assets/6c702d8f-0121-475a-8b99-55681761fbba" />

<br>

**Histogram**
<br>
```
x=[2, 1, 3, 4, 6, 2, 6, 3, 9, 4, 6, 5, 7, 2, 8, 2, 1, 8, 3, 4, 6, 7, 4, 5, 4, 6, 3, 9, 6, 10, 10, 9, 4]
plt.hist(x,bins=10,color='green',alpha=0.5)
plt.show()
```

<img width="865" height="501" alt="Hist" src="https://github.com/user-attachments/assets/b67c7300-f44e-446b-94bc-279841bda8dd" />

<br>

**Box Plot**
<br>
```
import numpy as np
np.random.seed(0)
data = np.random.normal(loc=0,scale=1,size=100)
data
fig, ax = plt.subplots()
ax.boxplot(data)
ax.set_xlabel("Data")
ax.set_ylabel("Values")
ax.set_title("Box Plot")
plt.show()
```

<img width="690" height="679" alt="Box" src="https://github.com/user-attachments/assets/929d5488-eff2-4148-9ddc-f94b428161cb" />

<br>


# Result:
 Thus, all the data visualization techniques of matplotlib has been implemented.
