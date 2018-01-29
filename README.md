## CSX450-1_Final-Exam

### Abalone Data Set

#### Overview
Abalone is a common name for marine snails. They have a highly iridescent inner shell, which gives it a range of changeable colors. Their meat is often used for food and the shells are used as decorative items or for jewelry. The goal of this data set is to predict the age of abalone from their physical measurements. Here is a quick summary of this problem set:

- Domain: Life/ Biology  
- Problem Statement: Predict the age of abalone from physical measurements  
- Description of Dataset: 4177 instances with 9 attributes (sex, length, diameter, height, weight, etc.)  
- Solution: Linear Regression  
- Benchmark Model: Divide the dataset into 50%   
- Performance Metric: Mean Squared Error  

#### 1. Domain

This dataset observed abalone, which is part of the life & biology domain. It comes from an original study in "The Population Biology of Abalone in Tasmania" by Warwick Nash, Tracy Sellers, Simon Talbot, Andrew Cawthorn, and Wes Ford. The dataset was donated by the Marine Resources Division in the Marine Research Laboratories of Taroona. Today, it is found in the the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/abalone).

#### 2. Problem Statement

The goal of this dataset is to predict the age of abalone from its physical measurement. The age of abalone is determined by cutting the shell through the cone, staining it, and counting the number of rings through a microscope. This is a tedious and time-consuming task. With machine learning, one would be able to predict the age without all the physical labor.

#### 3. Description of Dataset

This dataset is 269528 bytes, or approxiamately 270 kB. This dataset has 9 attributes collected from a study on 4177 abalone. Variables include sex, length, diameter, height, whole weight, shucked weight, viscera weight, shell weight, and number of rings. The last attribute, number of rings, is the attribute to predict, either as a continuous value or as a classification problem. This value represents the age of the abalone.

```{r}
'data.frame':	4177 obs. of  9 variables:
 $ sex           : Factor w/ 3 levels "F","I","M": 3 3 1 3 2 2 1 1 3 1 ...
 $ length        : num  0.455 0.35 0.53 0.44 0.33 0.425 0.53 0.545 0.475 0.55 ...
 $ diameter      : num  0.365 0.265 0.42 0.365 0.255 0.3 0.415 0.425 0.37 0.44 ...
 $ height        : num  0.095 0.09 0.135 0.125 0.08 0.095 0.15 0.125 0.125 0.15 ...
 $ whole_weight  : num  0.514 0.226 0.677 0.516 0.205 ...
 $ shucked_weight: num  0.2245 0.0995 0.2565 0.2155 0.0895 ...
 $ viscera_weight: num  0.101 0.0485 0.1415 0.114 0.0395 ...
 $ shell_weight  : num  0.15 0.07 0.21 0.155 0.055 0.12 0.33 0.26 0.165 0.32 ...
 $ rings         : int  15 7 9 10 7 8 20 16 9 19 ...
```

![Abalone Pairs](https://user-images.githubusercontent.com/22715593/35540539-37e37dea-050b-11e8-8bbc-009baf172f24.JPG)

#### 4. Solution 

The scatterplots show linear relationships between pairs of attributes. A solution to this problem is to perform a linear regression.   

#### 5. Benchmark Model

To test the regression, a suitable benchmark model is to run a simple trial by splitting the data in half.

#### 6. Performance Metric 

This model can be evaluated by using the Mean Squared Error.
