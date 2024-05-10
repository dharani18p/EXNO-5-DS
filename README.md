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
x_val = [0,1,2,3,4,5]
y_val = [0,1,4,9,16,25]
plt.plot(x_val,y_val)
plt.show()
```
![326323870-c3b1567c-eda6-46f9-97c0-5edcbc751613](https://github.com/dharani18p/EXNO-5-DS/assets/118343366/cf95bb4f-98e3-4e0c-b346-1b0bceb4d0d1)

```
import matplotlib.pyplot as plt
x = [1,2,3]
y = [2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My first graph')
plt.show()
```
![326323898-0e9fe2e2-0d99-4f7e-bdb7-85543ac9252b](https://github.com/dharani18p/EXNO-5-DS/assets/118343366/b89a2096-b372-4438-94df-dd7257111a00)

```
import matplotlib.pyplot as plt
x1 = [1,2,3]
y1 = [2,5,3]
plt.plot(x1,y1,label = 'line 1')
x2 = [1,2,3]
y2 = [3,1,6]
plt.plot(x2,y2,label = 'line 2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("Two lines on the same graph")
plt.legend()
plt.show()
```
![326323923-7678c654-4c38-4d56-9739-82c396ee8ada](https://github.com/dharani18p/EXNO-5-DS/assets/118343366/c3cf08fd-d01b-492e-a371-6c5700a580d1)

```
import matplotlib.pyplot as plt
import numpy as np
x = [1,2,3,4,5]
y1 = [10,12,14,16,18]
y2 = [5,7,9,11,13]
y3 = [2,4,6,8,10]
plt.fill_between(x,y1,color = 'blue')
plt.fill_between(x,y2,color = 'orange')
```
![326323942-73207267-25b7-4d47-8ddc-8de6c259faa8](https://github.com/dharani18p/EXNO-5-DS/assets/118343366/b32d98eb-5f1e-47eb-a6a7-1f172937205b)

```
plt.stackplot(x,y1,y2,y3,labels = ['line1','line2','line3'])
plt.legend(loc = 'upper left')
plt.title('Stacked line charts')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
![326323981-85a5c274-6f3c-4644-916f-8911a32ab070](https://github.com/dharani18p/EXNO-5-DS/assets/118343366/b348c97d-d44f-4860-84c9-7eb93d9eb103)

```
import numpy as np
import matplotlib.pyplot as plt
val = [2,4,7,3]
names = ['A','B','C','D']
plt.bar(names, val,color = 'purple')
plt.show()
```
![326324010-bbef76a4-0018-454e-81af-c4c29f91cc01](https://github.com/dharani18p/EXNO-5-DS/assets/118343366/d22f1e0a-f14b-4d92-8339-b4c5478eb6f6)

```
import matplotlib.pyplot as plt
import numpy as np
ages = [2,6,4,12,13,12,16,18,18,19,26,24,39,34,45,42,54,56,90,56,86,79]
range = (0,100)
bins = 10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no of people')
plt.title('histogram')
plt.show()
```
![326324408-45c9d44d-536f-4d4b-a30a-a1556a5e4762](https://github.com/dharani18p/EXNO-5-DS/assets/118343366/e63577e6-5051-4beb-896a-652d6cce09e0)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![326324171-57013638-cf5c-4384-807d-a5ae720fac62](https://github.com/dharani18p/EXNO-5-DS/assets/118343366/66454d5b-c4a5-4f16-b993-412d2f55f4b9)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel("data")
ax.set_ylabel("values")
ax.set_title("box plot")
```
![326324369-c1307c5c-99e4-4e67-b0a0-2a59ef9eecc6](https://github.com/dharani18p/EXNO-5-DS/assets/118343366/d983dc38-adb1-4afe-89ee-c0887008a7bb)

```
import matplotlib.pyplot as plt
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels = slices,colors=colors,startangle=90,shadow = True,explode = (0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
![326324333-aff6791e-db9d-4bff-8f4a-6ee9444d5913](https://github.com/dharani18p/EXNO-5-DS/assets/118343366/8335a4cd-2033-43da-b056-a88cb1102ac8)


# Result:
  Thus, We have successfullu performed Data Visualization using matplot python library for the given datas.
