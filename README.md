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
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.plot(x_values,y_values)
plt.show()
```
![Screenshot 2024-05-04 090705](https://github.com/Harsayazheni/Expt05-Introduction-to-Data-Science/assets/118708467/30e9f541-c170-42df-82e3-b1643cc8898d)

```
import matplotlib.pyplot as plt
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel("y-axis")
plt.title('My first grpah!')
plt.show()
```
![Screenshot 2024-05-04 090714](https://github.com/Harsayazheni/Expt05-Introduction-to-Data-Science/assets/118708467/f3588270-037c-4db1-b08e-e8c6001dc90f)

```
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line 1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line 2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("two lines on same grapg!")
plt.legend()
plt.show()
```
![Screenshot 2024-05-04 090722](https://github.com/Harsayazheni/Expt05-Introduction-to-Data-Science/assets/118708467/aaa5b396-1492-478e-ab54-8166cc778fff)

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
![Screenshot 2024-05-04 090730](https://github.com/Harsayazheni/Expt05-Introduction-to-Data-Science/assets/118708467/ee1784f8-1d73-41c1-b4b4-cd74107b5294)

```
plt.stackplot(x,y1,y2,y3,labels=['line1','line2','line3'])
plt.legend(loc='upper left')
plt.title('stacked line chart')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
![Screenshot 2024-05-04 090739](https://github.com/Harsayazheni/Expt05-Introduction-to-Data-Science/assets/118708467/bb7f11dc-d884-41ef-9561-bb6ae87994fd)

```
import numpy as np
import matplotlib.pyplot as plt
values=[5,6,3,7,2]
names=["A","B","C","D","E"]
plt.bar(names,values,color='green')
plt.show()
```
![Screenshot 2024-05-04 090746](https://github.com/Harsayazheni/Expt05-Introduction-to-Data-Science/assets/118708467/25e437eb-08d1-4a52-966e-348702bcf84c)

```
import matplotlib.pyplot as plt
import numpy as np

ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range = (0, 100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no of people')
plt.title('histogram')
plt.show()
```
![Screenshot 2024-05-04 090756](https://github.com/Harsayazheni/Expt05-Introduction-to-Data-Science/assets/118708467/9654fb4b-87d7-4898-98f9-85bd41c592f6)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![Screenshot 2024-05-04 090805](https://github.com/Harsayazheni/Expt05-Introduction-to-Data-Science/assets/118708467/b7c7a258-5d38-4395-b128-e0382454afbb)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel("data")
ax.set_ylabel("values")
ax.set_title("box plot")
```
![Screenshot 2024-05-04 090814](https://github.com/Harsayazheni/Expt05-Introduction-to-Data-Science/assets/118708467/909124d3-b53e-4100-b660-bae565df861e)

```
import matplotlib.pyplot as plt
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels = slices,colors=colors,startangle=90,shadow = True,explode = (0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
![Screenshot 2024-05-04 090823](https://github.com/Harsayazheni/Expt05-Introduction-to-Data-Science/assets/118708467/ead7a686-92a6-4a1a-80c5-e789ab8e0e05)


# Result:
The Data Visualization using matplot python library is implemented successfully.
