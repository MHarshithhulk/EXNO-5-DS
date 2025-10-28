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
 Include the necessary coding and corresponding screenshots
'''

import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt

# Line Plot:
'''

marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()

'''

<img width="1132" height="727" alt="image" src="https://github.com/user-attachments/assets/dc0db22e-bf15-4dc8-8ab5-ad951da8c68c" />

'''

student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()

'''
<img width="1042" height="751" alt="image" src="https://github.com/user-attachments/assets/4f4ee17e-63ca-4941-86f7-0365f05fa867" />

# Scatter Plot:

'''

x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()

'''

<img width="852" height="657" alt="image" src="https://github.com/user-attachments/assets/cc3d3a5e-4f36-41f8-b8a3-4c3d8499e422" />

'''

x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()

'''
<img width="862" height="835" alt="image" src="https://github.com/user-attachments/assets/4f578b4d-2c8e-4640-a375-6c0102860d4e" />

# Pie Chart:

'''

act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()

'''

<img width="1357" height="707" alt="image" src="https://github.com/user-attachments/assets/42f8b8cd-a033-4af6-8179-4de3243784aa" />

'''

feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()

'''

<img width="1477" height="687" alt="image" src="https://github.com/user-attachments/assets/068d371a-6050-4af1-9ea3-266a0da4a970" />

# Area Chart:

'''

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

'''

<img width="935" height="823" alt="image" src="https://github.com/user-attachments/assets/2eb5724b-3140-43e5-9d31-336607240761" />

# Bar Chart:

'''

height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green']
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()

'''

<img width="917" height="823" alt="image" src="https://github.com/user-attachments/assets/5ae6a63f-8adb-48d6-b6c0-5a68b8901220" />

# Histogram:

'''

x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()

'''

<img width="808" height="635" alt="image" src="https://github.com/user-attachments/assets/4218ee5a-2ede-436f-ad98-3c53d9316dd3" />

# Box Plot:

'''

np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data

'''

<img width="845" height="551" alt="image" src="https://github.com/user-attachments/assets/29cb7a1b-663f-4a9c-891b-0ba8a2944d52" />

'''

fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')

'''

<img width="825" height="783" alt="image" src="https://github.com/user-attachments/assets/0c4db929-2d72-4289-bd16-eb2b72284940" />



# Result:
Thus the program to Perform Data Visualization using matplot python library for the given datas is been implemented.
