# Individual programming assignment

In this assignment you will work on your own. You should choose **one** of the problems listed below and code up a solution in R or Python. You are not allowed to use any of the functions from the packages that have already coded up these algorithms. I will evaluate your submission based on correctness of the implementation and how well the code is written. Please make sure your solution is reproducible and platform independent, I should be able to rerun your code and obtain your results/figures with a single line command. 

You should be able to find the references mentioned in the text on the Internet. Books are available free of charge on authors' websites.

Deadline is **May 31, 23:59**


## 1.  Bernoulli bandit problem

This problem focuses on strategies for making choices and illustrates the exploration-exploitation trade-off that is unique to reinforcement learning. In Bayesian optimization these choice strategies are often called acquisition functions (e.g. Shahriari etal 2016, pg 160).

You will program agents whose task is to perform well in a Bernoulli bandit problem with K arms where the best arm has a reward probability of 0.5 and the K − 1 other arms have a probability of 0.5 − ε.  

You will program the following four agents.  
a) ε-Greedy (see Sutton & Barto, 1998, chapter 2)  
b) Softmax (see Sutton & Barto, 1998, chapter 2)    
c) UCB1 (see Auer 2002, pg 237)  
d) Thompson sampling (see Shahriari etal 2016, pg 152)  

You can use my handouts for these agents/algorithms, but I have listed some useful references where you can find more details about them. For the learning component you can use either simple means, or online learning/updating rule (you can play a bit with learning rate parameter, trying to find a good value), or use Bayesian updating with a Beta-Bernoulli model (set the priors to uniform). Note that for UCB1 you will have to force sampling of each option before starting to use the choice rule (initialization part of the algorithm).

You should compare performance of your four agents in four versions of the problem specified above, where K ∈ {10, 100} and ε ∈ {0.02, 0.1}. For each version of the problem present a single plot with the performance of all four algorithms expressed as cumulative regret (y-axis) over log-transformed time (x-axis). This makes four figures in total. You will need to simulate agents for at least 100000 steps/trials to get good trends and run about 100 simulations to get more reliable estimates for each agent. 

This is the minimum, feel free to investigate other behaviours of the algorithms.  


## 2. Basic Gaussian process algorithm

This problem focuses on Gaussian process, supervised learning algorithm that is most often used as a function learning component of Bayesian optimization algorithm (e.g. Shahriari etal 2016, pg 157).

You will program the Gaussian process algorithm with constant mean function and two types of kernels:  
a) Linear kernel (equivalent to Bayesian linear regression)  
b) Squared exponential kernel  

I recommend reading chapter 2 of Rasmussen and Williams (2006) for this, my slides are unlikely to be enough for coding up this algorithm.

Using one-dimensional data, do the following:  
- Choose some hyperparameter values and draw some sample functions from the prior. Illustrate this for both types of kernels (this should look like Figure 2.2 a/ in the chapter 2). This should result in two figures, one for each kernel.   
- Explore how functions change as you change the hyperparameters. Choose a new set of hyperparameters for each kernel and repeat the previous exercise. This should result in two figures, one for each kernel.   
- Create two interesting one-dimensional functions and generate five input-output pairs of observations for each of them.   
- For the two kernels and two sets of hyperparameters defined in the previous exercises update the priors with the five observations and make some draws from the posterior. Illustrate this in figures, together with predictive mean and variance of the posterior (see Figure 2.2 b/ and Figure 2.5 in chapter 2). You should have one figure for each combination of kernel, hyperparameter set and function, eight in total.   

This is the the required part, feel free to investigate other behaviours of the algorithms.  


## References

Auer, P., Cesa-Bianchi, N., & Fischer, P. (2002). Finite-time analysis of the multiarmed bandit problem. Machine Learning, 47, 235–256. 

Rasmussen, C. E., & Williams, C. K. I. (2006). Gaussian processes for machine learning. MIT Press.

Shahriari, B., Swersky, K., Wang, Z., Adams, R. P., & de Freitas, N. (2016). Taking the Human Out of the Loop: A Review of Bayesian Optimization. Proceedings of the IEEE, 104(1), 148–175. http://doi.org/10.1109/JPROC.2015.2494218

Sutton, R. S., & Barto, A. G. (1998). Reinforcement learning: An introduction. Cambridge, MA, US: MIT Press.  
