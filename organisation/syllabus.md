# Topics in Big Data Analytics II - Bayesian optimization

Lecturer: Hrvoje Stojić, University College London and BGSE


## Overview and Objectives

Bayesian optimization is a framework for modelling situations where one wants to learn functions in a supervised manner, but also smartly select inputs with the idea of making the maximization more efficient. Related ideas can be found in other fields of machine learning and statistics, such as active learning or optimal experimental design. This framework has been used in modelling autonomous agents and solving certain types of reinforcement learning problems, but its usage recently blossomed due to applications in optimizing (hyper)parameters of models that are costly to evaluate. Use-cases include optimizing the hyperparameters of deep neural networks or optimizing parameters of scheduling and planning optimizers that have a long runtime. The objective of the course is to provide you with a basic understanding of the theory behind the Bayesian optimization, and equip you with sufficient amount of know-how to immediately incorporate it into your workflow and substitute less efficient grid-search methods. Bayesian optimization is a general framework and we will illustrate other use-cases.



## Course Outline

We will first briefly introduce the reinforcement learning problem and distinguish it from other types of machine learning problems, providing an overview of basic concepts, such as multi-armed bandit problems or exploration-exploitation trade-off. We will spend more time on basics of the Gaussian processes - great supervised learning method which gives you the full Bayesian non-parametric treatment. We will focus on regression problems and you will learn how to deploy Gaussian processes in practice.

Next we will examine contextual multi-armed bandit problem in more details and uncertainty-based decision strategies for balancing the exploration-exploitation trade-off. Together with Gaussian processes this will allow us to formulate the Bayesian optimization algorithm and illustrate some of its many potential uses. We will focus on one particular use case - you will learn how to use it for optimizing hyper-parameters.



## Required Activities

Attendance to theory classes, individual problem set and group project.


## Evaluation

One individual problem set (40%) and one group-based project (60%). 


## Materials

Rasmussen, C. E., & Williams, C. K. I. (2006). Gaussian processes for machine learning. MIT Press.

Shahriari, B., Swersky, K., Wang, Z., Adams, R. P., & de Freitas, N. (2016). Taking the Human Out of the Loop: A Review of Bayesian Optimization. Proceedings of the IEEE, 104(1), 148–175. http://doi.org/10.1109/JPROC.2015.2494218

Snoek, J., Larochelle, H., & Adams, R. P. (2012). Practical Bayesian Optimization of Machine Learning Algorithms. In Advances in Neural Information Processing Systems (pp. 2951–2959). http://doi.org/2012arXiv1206.2944S


