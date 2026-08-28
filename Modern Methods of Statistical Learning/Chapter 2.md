The book will only handle supervised learning.

For each problem, there are measured or preset variables called *inputs*. These variables have some influence on the *outputs*. The outputs can be *quantitative* if the output is some kind of measurment like on a floating scale of 1-10. On the other hand, the output is *qualitative* if it assumes values in a finite set. There is also a third one calledd *ordered categorical* which is like a qualitative one but a definitive order exists between them.

The prediction tasks are split up depending on the output type. *Regression* is when we predict quantitative outputs and *classification* when we predict qualitative outputs. 

Input variables are denoted with $X$, if a vector its components are $X_{j}. $Observed variables are denoted with smaller case, the $i$th  observed value of $X$ is $x_{i}$. Bold letters are used for matrices. Like a set up $N$ input $p$-vectors are represented as a $N \times p$ matrix $\mathbf{X}$. Outputs are denoted by $\hat{Y}$. 

We assume we have available a set of training data $(x_{i}, y_{i})$, $i=1,\dots ,N$ with which we will construct our prediction rule.
## Linear Models and Least Squares
Given a vector of inputs $X^T = (X_{1}, X_{2},\dots,X_{p})$, we predict $Y$ via the model
$$
\hat{Y} = \hat{\beta}_0 + \sum_{j=1}^{p} X_j \hat{\beta}_j.
$$
where $\hat{\beta}_{0}$ is the intercept. 