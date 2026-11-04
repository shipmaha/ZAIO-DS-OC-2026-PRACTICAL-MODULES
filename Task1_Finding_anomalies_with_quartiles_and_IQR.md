Task 1: Finding anomalies with quartiles and IQR
Provide evidence, then save before moving on.

1.1 – In your own words, provide an explanation of what quartiles are. (1 mark)

quartiles are values that divide ordered dataset into four equal parts

1.2 – What does the formula k(n+1)/4 calculate. (1 mark)

it calculates the position of the kth quartile in the ordered/sorted dataset

1.3 – If the formula k(n+1)/4 returns a non-integer m, what should you do? (1 mark)

interpolate between the values at the positions on either side of m. For example at position 3.25 take one quarter of the distance from the 3rd value to the 4th value.


Assume the following dataset is the test scores of a class of students

9 44 45 46 48 50 53 55 60 61 99 100



1.4 – What position is Quartile 1 in? (1 mark)

k(n+1)/4 = 1 × (12+1)/4 = 13/4 = 3.25

1.5 – What is the value of Quartile 1? (1 mark)

The 3rd and 4th scores are 45 and 46. interpolating at position 3.25 so Q1 = 45 + 0.25(46 - 45) = 45.25

1.6 – What is the value of Quartile 2? (1 mark)

Q2 position 2(12 + 1)/4 = 6.5. Q2 = 50 + 0.5 * (53 − 50) = 50 + 1.5 = 51.5

1.7 – What is the value of Quartile 3? (1 mark)

Q3 position 3(12 + 1)/4 = 9.75. Q3 = 60 + 0.75 × (61 − 60) = 60 + 0.75 = 60.75

1.8 – Provide the value of the Interquartile Range. (1 mark)

IQR = Q3 - Q1 = 60.75 - 45.25 = 15.5.

1.9 – Provide the value of the Lower Bound and the Upper Bound. (1 mark)

Lower bound = Q1 - 1.5 * IQR = 45.25 - 1.5 * 15.5 = 45.25 - 23.25 = 22.
Upper bound = Q3 + 1.5 * IQR = 60.75 + 1.5 * 15.5 = 60.75 + 23.25 = 84.

1.10 – Provide all the values that are outliers in this dataset. If none exist, provide a value that would have been an outlier. (1 mark)

Scores below 22 or above 84 are outliers. 9, 99, and 100 are outliers


Task 2: Finding anomalies with z-scores
2.1 – Given two data sets, A = [50, 50, 50, 50] and B = [20, 40,60,80], which dataset will have a higher variance value? (1 mark)

dataset B has the higher variance. dataset A has no variance all are identical variance = 0, while the values in B differ from one another and are spread far from the mean


Use the following sample data to answer the questions below

12 15 18 20 22 25 27 30 31 35 36 40



2.2 – Calculate the mean for the above dataset. (1 mark)

Mean = (12 + 15 + 18 + 20 + 22 + 25 + 27 + 30 + 31 + 35 + 36 + 40)/12 = 311/12 = 25.9167 

2.3 – Calculate the variance of the sample data. (1 mark)

(12−25.9167)^2 = 193.67
(15−25.9167)^2 = 119.17
(18−25.9167)^2  62.67
(20−25.9167)^2 = 35.01
(22−25.9167)^2 = 15.34
(25−25.9167)^2 = 0.84
(27−25.9167)^2 = 1.17
(30−25.9167)^2 = 16.67
(31−25.9167)^2 = 25.84
(35−25.9167)^2 = 82.51
(36−25.9167)^2 = 101.67
(40−25.9167)^2 = 198.34
Sum of squared deviations = 852.92
Sample variance = 852.92 / (12 − 1) = 852.92 / 11 = 77.54

2.4 – Provide the standard deviation for the above sample dataset. (1 mark)

standard deviation = square root of 77.54 = 8.81

2.5 – Given a dataset with the mean μ = 21 and a standard deviation 𝜎 = 2.33, is x = 32.184 an anomaly based on its z-score? (1 mark)

z = (x - μ)/σ = (32.184 - 21)/2.33 = 4.8. Yes it is an anomaly, its z-score is well beyond 3 standard deviations from the mean