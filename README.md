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
~~~
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1, y1, label='line 1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2, y2, label='line 2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph')
plt.legend()
~~~
![image](https://github.com/user-attachments/assets/e37731ae-9f7e-4094-84b0-51057c8216d2)
~~~
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y, color='blue', linestyle='dashed', linewidth=3, marker='o', markerfacecolor='red', markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customization')
~~~
![image](https://github.com/user-attachments/assets/677c4171-7ae3-431e-85c6-0a177e03a82b)
~~~
years=range(2000, 2012)
apples=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931, 0.934, 0.936, 0.937, 0.9375, 0.9372, 0.939]
oranges=[0.962, 0.941, 0.930, 0.923, 0.918, 0.908, 0.907, 0.904, 0.901, 0.898, 0.9, 0.896]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectre)')
plt.title('Crops yield in Kento')
plt.legend(['Apples', 'Oranges'])
~~~
![image](https://github.com/user-attachments/assets/c7b647c8-8f9e-4a85-9498-4e87b03c3467)
~~~
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
~~~
![image](https://github.com/user-attachments/assets/73b1735d-9a5b-4ff6-8f7f-f38ab9b2af4b)
~~~
import numpy as np
np.pi
~~~
![image](https://github.com/user-attachments/assets/32dbf630-219e-407b-92f8-ec14b9842192)
~~~
x=np.arange(0,4 * np.pi, 0.1)
y=np.sin(x)
plt.title('Sine Wave form')
plt.plot(x,y,'g--', linewidth=3)
~~~
![image](https://github.com/user-attachments/assets/5c894d84-0450-41cf-8a2d-b6a0107d7263)
~~~
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='pink')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
~~~
![image](https://github.com/user-attachments/assets/638c28d0-aec3-4733-afc1-f70288ed85d6)
~~~
plt.stackplot(x,y1,y2,y3,labels=['Line1','Line2', 'Line3'])
plt.legend(loc='upper left')
plt.title('Stacked Line Chart')
plt.xlabel('X-axis')
plt.xlabel('Y-axis')
~~~
![image](https://github.com/user-attachments/assets/e790adc8-571f-4e8c-87a4-0a0ced4c4733)
~~~
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar Graph')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
~~~
![image](https://github.com/user-attachments/assets/4127253a-4129-45af-bd3c-dc265bd87f62)
~~~
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
~~~
![image](https://github.com/user-attachments/assets/151d8231-c701-4132-bff2-2b95198bd275)
~~~
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,80,19,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no. of. people')
plt.title('My Histogram')
~~~
![image](https://github.com/user-attachments/assets/b5ac8600-8ba4-4181-a102-8f81a76ed491)
~~~
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10, color='blue',alpha=0.5)
~~~
![image](https://github.com/user-attachments/assets/3dc76151-15a7-4520-8bfc-52c579145e8f)
~~~
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
~~~
![image](https://github.com/user-attachments/assets/7a3d177c-c976-4a8d-a11d-9be62aa7f666)
~~~
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
~~~
![image](https://github.com/user-attachments/assets/9a950f6d-bb1c-4194-9261-f5fb888f3900)
~~~
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
~~~
![image](https://github.com/user-attachments/assets/2e094920-5945-4998-814e-5dd2b5d444ff)
~~~
labels='Python', 'C++', 'Ruby', 'Java'
sizes=[215, 130, 245, 210]
colors=['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
~~~
![image](https://github.com/user-attachments/assets/5a7d168c-9e81-48e1-bce0-6d905877a8c0)


# Result:
 Thus Data Visualization using matplot python library for the given datas was executed successfully.
