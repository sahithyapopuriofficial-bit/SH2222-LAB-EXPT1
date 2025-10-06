# Experiment 1: Exponential Distribution analysis using Python 

**Question:**

Write a Python program to generate random data from an Exponential distribution and 
calculate its mean and variance. Plot the histogram of the data.

**Aim:**  

To generate random numbers from an Exponential distribution, calculate their mean and 
variance, and visualize the data using a histogram. 

**Software Required:**  

Python and Libraries - numpy and matplotlib

**Procedure:**   

**Mathematical Explanation:** 

 <img width="674" height="160" alt="{9AA55CC6-54DF-472A-8C9D-31CF3D79BB03}" src="https://github.com/user-attachments/assets/bce7c45a-a316-46ee-aaf6-777474ea4506" />

**Steps in Python:**  
1. Import numpy and matplotlib  (for mathematical operations and graph) 
2. Use numpy.random.exponential(scale,size) to generate data. Here scale (1/𝜆) 
3. Calculate mean using numpy.mean(data) and variance using numpy.var(data). 
4. Plot histogram with matplotlib.pyplot.hist() to visualize the shape of the distibution.  
5. Display the numerical results and the graph.

**PROGRAM**
```
import numpy as np 
import matplotlib.pyplot as plt 
# Generate random data from Exponential distribution 
data = np.random.exponential(scale=5, size=1000) 
# Calculate mean and variance 
mean = np.mean(data) 
variance = np.var(data) 
print("Mean:", mean) 
print("Variance:", variance) 
# Plot histogram 
plt.hist(data, bins=10, color='lightgreen', edgecolor='black') 
plt.title("Exponential Distribution") 
plt.xlabel("Value") 
plt.ylabel("Frequency") 
plt.show()
```

**OUTPUT**

<img width="742" height="614" alt="{F51B5AFC-5620-4B31-A811-EC557F2A38F0}" src="https://github.com/user-attachments/assets/bd9a37f9-ca51-4ca9-a99b-8f9adaf1a343" />

**RESULT:**

The program successfully generated random data from an Exponential distribution, calculated 
its mean and variance, and plotted the histogram. 
