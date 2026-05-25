#  Mean and variance of a discrete  distribution
reg no:212225040404
name:sharmila
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

# Input values (arrival of objects)
x = [0, 1, 2, 3, 4]

# Corresponding frequencies
f = [5, 10, 15, 10, 5]

# Total frequency
N = sum(f)

print("Total Frequency (N) =", N)

# Probability Distribution
p = []
print("\nProbability Distribution:")
print("x\tf\tP(x)=f/N")

for i in range(len(x)):
    prob = f[i] / N
    p.append(prob)
    print(f"{x[i]}\t{f[i]}\t{prob:.4f}")

# Mean Calculation
mean = 0
print("\nCalculation of Mean:")
print("x\tP(x)\tx*P(x)")

for i in range(len(x)):
    xp = x[i] * p[i]
    mean += xp
    print(f"{x[i]}\t{p[i]:.4f}\t{xp:.4f}")

print("\nMean =", round(mean, 4))

# Variance Calculation
variance = 0
print("\nCalculation of Variance:")
print("x\tP(x)\t(x-Mean)^2\tP(x)*(x-Mean)^2")

for i in range(len(x)):
    term = ((x[i] - mean) ** 2)
    vp = p[i] * term
    variance += vp
    print(f"{x[i]}\t{p[i]:.4f}\t{term:.4f}\t\t{vp:.4f}")

print("\nVariance =", round(variance, 4))
```
# Output : 
<img width="228" height="331" alt="image" src="https://github.com/user-attachments/assets/506693d0-1bb1-4c12-8d0a-0f5e132f0f4b" />


