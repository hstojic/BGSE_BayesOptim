# Individual Problem Set

## 1.  Bernoulli bandit problem

Your agent faces a Bernoulli bandit problem with K arms where the best arm has a reward probability of 0.5 and the K − 1 other arms have a probability of 0.5 − ε. 

You will program the following four agents:  
a) ε-Greedy  
b) Softmax   
c) UCB1  
d) Thompson Beta-Bernoulli  

Use the online version of the learning/update rule (play a bit with learning rate parameter, try to find a good value), and set the initial Q-values to zero. For UCB1 you will have to force sampling of each option before starting to use the choice rule. For Beta-Bernoulli set the prior to uniform (but play a bit with setting the prior).

Compare performance of your four agents in four versions of the problem specified above, where K ∈ {10, 100} and ε ∈ {0.02, 0.1}. I would like to see their performance expressed as cumulative regret in function of time. you should simulate each agent about 100 times to get more reliable estimates. This is the minimum, feel free to investigate other behaviours of the algorithms.  


## 2. Basic Gaussian process algorithm

You should code the Gaussian process algorithm with constant mean function and Gaussian kernel with ARD. Choose some initial GP hyperparameter values, draw some sample functions from the prior and illustrate them in a figure. Create 3 interesting 1-dimensional functions and generate 5 input-reward pairs of observations for each of them. Optimize the hyperparameters given these 5 observations (no need to be very careful about the learning algorithm here), update the posterior, make some draws from the posterior and illustrate them in a figure. Do this for each of the three functions. On the figures always illustrate the estimated mean and variance of the distribution.  


## Evaluation

I expect a report with the results of the analysis and the code written in R. I will evaluate your problem set based on correctness of the implementation, how well the code is written and the report. You are not allowed to use any of the functions from the packages that have already coded up these algorithms.

