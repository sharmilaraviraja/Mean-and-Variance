#  Mean and variance of a discrete  distribution


# Aim : 

To find mean and variance of arrival of objects from the feeder using probability distribution


# Software required :  

Python and Visual components tool

# Theory:

The expectation or the mean of a discrete random variable is a weighted average of all possible
values of the random variable. The weights are the probabilities associated with the corresponding values. 
It is calculated as,

![image](https://user-images.githubusercontent.com/103921593/192938463-e34177f4-f188-48a0-bda2-8f6d1d660ed2.png)

The variance of a random variable shows the variability or the scatterings of the random variables.
It shows the distance of a random variable from its mean. It is calcualted as

![image](https://user-images.githubusercontent.com/103921593/192938695-99fedc01-34d5-4d36-84df-5880e766ed0c.png)


# Procedure :

1. Construct frequency distribution for the data

2. Find the  probability distribution from frequency distribution.

3. Calculate mean using 
   
   ![image](https://user-images.githubusercontent.com/103921593/192940431-03b81777-c54d-4286-b4f4-82dfe7666b4c.png)

4. Find  
   
      ![image](https://user-images.githubusercontent.com/103921593/192940255-2d9dd746-6875-4a6d-877b-6da6cdb96ab1.png)

5.  Calculate variance using 
  
      ![image](https://user-images.githubusercontent.com/103921593/192942852-913550a9-fabe-4a55-b956-0487b18bbd97.png)


# Experiment :

![image](https://user-images.githubusercontent.com/103921593/229993174-5b67e57e-3e01-4ac4-9f83-410a932b22bf.png)

# Program :
```
# Mean and Variance of a Discrete Distribution

# Input values of random variable X
x = [0, 1, 2, 3, 4]

# Corresponding probabilities P(X)
p = [0.1, 0.2, 0.3, 0.25, 0.15]

# Calculate Mean
mean = 0
for i in range(len(x)):
    mean = mean + (x[i] * p[i])

# Calculate E(X^2)
ex2 = 0
for i in range(len(x)):
    ex2 = ex2 + ((x[i] ** 2) * p[i])

# Calculate Variance
variance = ex2 - (mean ** 2)

# Display results
print("Discrete Probability Distribution")
print("--------------------------------")
print("X :", x)
print("P(X) :", p)

print("\nMean =", mean)
print("Variance =", variance)
```


# Output : 
<img width="391" height="164" alt="image" src="https://github.com/user-attachments/assets/6659b83b-290f-4a4e-b77f-f0cb8fc46c31" />

# Results :
The mean and variance of arrivals of objects from feeder using probability distribution are calculated.

