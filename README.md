# One Sample Stochastic Subspace Frank Wolfe

## Introduction
Repository for EE698U course project (Big Data Convex Optimization, IIT Kanpur), on proposed variants of Frank Wolfe in Stochastic settings for strongly convex functions in compact set.

## Abstract
The advantage of using projected gradient descent is its simple projecting operator which solves the minimizing problem off-grid. 

It becomes quite stable and fast in the stochastic setting which has been widely used in machine learning applications. 

However, projection-free algorithms are faster than Projection Gradient descent particularly Frank Wolfe Algorithm as it solves the problem linearly. 

Recently it has also been shown that even in a stochastic setting Frank-Wolfe can get optimal results in just one stochastic sample [1]. 

On a different note, there have been works in improving per iterate time complexity as in the Subspace Stochastic Descent [2] by carrying out updates in a lower dimension. 

Our aim in this paper is to incorporate this idea of update in the subspace into One sample stochastic Frank-Wolfe. By doing this, the per iterate time complexity will improve as the bottleneck step of Frank Wolfe will be carried out in a lower dimension making it faster. In this paper, we propose two different algorithms that can be used in an oblivious setting.

The first algorithm recovers the optimality convergence rate of $`O\sqrt{\frac{1}{T}} `$ with the same oracle i.e. $`math \nabla F \tilde (x_{t},z_{t}) `$. 

In the second algorithm proposed, the optimality rate can be recovered by making a reasonable choice of dimensionality reduction factor which has been shown in the experiments.

## References
[1] [Mingrui Zhang, Zebang Shen, Aryan Mokhtari, Hamed Hassani, Amin Karbasi: One Sample Stochastic Frank-Wolfe](https://arxiv.org/pdf/1910.04322)
[2] [David Kozak, Stephen Becker, Alizera Doostan, Luis Tenorio. Stochatic Subspace Descent](https://arxiv.org/pdf/1904.01145)
