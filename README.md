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

%matplotlib inline
import numpy as np
x=np.arange(0,10)
y=np.arange(11,21)
a=np.arange(40,50)
b=np.arange(50,60)
plt.scatter(x,y,c='g')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```

<img width="733" height="557" alt="image" src="https://github.com/user-attachments/assets/7eca445b-9b5b-49ee-913a-135f3cdd52ba" />

```
import matplotlib.pyplot as plt
import numpy as np

x=np.arange(0,10)
y=x*x
plt.plot(x,y,'r*',linestyle='dashed',linewidth=2, markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.show()
```
<img width="757" height="565" alt="image" src="https://github.com/user-attachments/assets/06bc0503-0820-4916-ab3e-1b80f40406fc" />

```
x = np.arange(1,11)
y = 3 * x + 5
plt.title("Matplotlib demo")
plt.xlabel("x axis caption")
plt.ylabel("y axis caption")
plt.plot(x,y)
plt.show()
```

<img width="752" height="565" alt="image" src="https://github.com/user-attachments/assets/f9b19225-c8ee-4e1d-87ff-5944f0ddb513" />

```
np.pi
```

<img width="192" height="32" alt="image" src="https://github.com/user-attachments/assets/a78d1ad4-a25a-45d2-b4ca-5349dee50285" />

```
# Compute the x and y coordinates for points on a sine curve
x = np.arange(0, 4 * np.pi, 0.1)
y = np.sin(x)
plt.title("sine wave form")

# Plot the points using matplotlib
plt.plot(x, y)
plt.show()
```

<img width="737" height="533" alt="image" src="https://github.com/user-attachments/assets/4583f364-22a6-4333-870c-ff66ab006999" />

```
#Subplot()
# Compute the x and y coordinates for points on sine and cosine curves
x = np.arange(0, 5 * np.pi, 0.1)
y_sin = np.sin(x)
y_cos = np.cos(x)

# Set up a subplot grid that has height 2 and width 1,
# and set the first such subplot as active.
plt.subplot(2, 1, 1)

# Make the first plot
plt.plot(x, y_sin, 'r--')
plt.title('Sine')

# Set the second subplot as active, and make the second plot.
plt.subplot(2, 1, 2)
plt.plot(x, y_cos, 'g--')
plt.title('Cosine')

# Show the figure.
plt.show()
```

<img width="733" height="538" alt="image" src="https://github.com/user-attachments/assets/f4e61170-a9f7-415b-bbfa-f9d7b7458bbe" />

```
x = [2,8,10]
y = [11,16,9]

x2 = [3,9,11]
y2 = [6,15,7]
plt.bar(x, y)
plt.bar(x2, y2, color = 'g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')

plt.show()
```

<img width="742" height="562" alt="image" src="https://github.com/user-attachments/assets/8d4c600d-f960-460c-b310-a7c26986dc20" />

```
data = [np.random.normal(0, std, 100) for std in range(1, 4)]

# rectangular box plot
plt.boxplot(data,vert=True,patch_artist=False);
plt.show()
```

<img width="715" height="515" alt="image" src="https://github.com/user-attachments/assets/11ee860f-3c0c-4898-8750-c9058a5c7fb5" />

```
data
```

<img width="812" height="427" alt="image" src="https://github.com/user-attachments/assets/3e9134a4-b36f-428b-99a6-fc59263243d9" />


```
# Data to plot
labels = 'Python', 'C++', 'Ruby', 'Java'
sizes = [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0.4, 0, 0, 0)  # explode 1st slice

# Plot
plt.pie(sizes, explode=explode, labels=labels, colors=colors,
autopct='%1.1f%%', shadow=False)

plt.axis('equal')
plt.show()
```

<img width="690" height="455" alt="image" src="https://github.com/user-attachments/assets/6cfc493e-3a05-4d85-b3db-08e7fc289516" />

# Result:
Thus Data Visualization using matplot python library for the given datas is performed.
