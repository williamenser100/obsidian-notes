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
where $\hat{\beta}_{0}$ is the intercept. Can be written in vector form by including the constant variable $1$ in $X$ and include $\hat{\beta}_{0}$ in the vector $\hat{\beta}$ as 
$$
\hat{Y}=X^T\hat{\beta}.
$$
#### Least squares
Choose the coefficients in the vector $\beta$ as to minimize 
$$
\text{RSS}(\beta) = \sum_{i=1}^{N}(y_i - x_i^T \beta)^2.
$$
or
$$
RSS(\beta) = (\mathbf{y} - \mathbf{X}\beta)^T(\mathbf{y} - \mathbf{X}\beta),
$$
where $\mathbf{X}$ is a $P\times n$ matrix with each row being an input vector and $\mathbf{y}$ is an $N$-vector of the outputs in the training set. By differentiating by $\beta$ we get 
$$
\mathbf{X}^{T}(\mathbf{y} - \mathbf{X}\beta) = 0.
$$
If $\mathbf{X}^T\mathbf{X}$ is nonsingular, then the unique solution is 
$$
\hat{\beta} = (\mathbf{X}^{\mathbf{T}}\mathbf{X})^{-1}\mathbf{X}^{\mathbf{T}}\mathbf{y},
$$
#### Nearest-Neigbour Methods
The $k$-nearest neigbour fit for $\hat{Y}$ is defined by finding the $k$ training points whose inputs are closest to $x$, then predict $\hat{Y}(x)$ as the average of their $y$ values.

$$
\hat{Y}(x) = \frac{1}{k} \sum_{x_i \in N_k(x)} y_i,
$$
## Statistical Decision Theory
Let $X \in \mathbb{R}^p$ denote a real value random input vector and $Y \in \mathbb{R}$ a real valued output vector. They have a joint distribution $\text{Pr}(X,Y)$. We seek $f(X)$ for predicting $Y$. 
Let $L(Y, f(X))$ be the *loss function* for penalizing errors in prediction, the most common one is the squared error loss
$$
L(Y, f(X)) = (Y-f(X))^2
$$
The expected prediction error is then 
$$
EPE(f) = E[(Y-f(X))^2] = \int [y - f(x)]^2 \Pr(dx, dy)
$$
which can be written as 
$$
\text{EPE}(f) = \text{E}_{X}\text{E}_{Y|X}\left([Y - f(X)]^2 | X\right)
$$
$$
f(x) = \text{argmin}_{c} \mathbb{E}_{Y|X}\left([Y-c]^2 | X = x\right).
$$
with the solution
$$
f(x) = E(Y|X=x)
$$
known as the *regression* function.

If the output is a categorical variable $G$, an estimate $\hat{G}$ assumes values in the set of possible classes $\mathcal{G}$. The loss function is represented by a $K\times K$ matrix $\mathbf{L}$, where $K=\text{card}(\mathcal{G})$. $\mathbf{L}$ will be zero on the diagonal and nonnegative elsewhere. A common way to define the loss function is for it to be zero on the diagonal and one for all misclassifications.
$$
\text{EPE}=\text{E}[L(G,\hat{G}(X))]
$$
which is taken against $Pr(G,X)$. We can write
$$
\text{EPE} = E_{x}\sum_{k=1}^KL[\mathcal{G}_{k}, \hat{G}(X)]\text{Pr}(\mathcal{G}_{k}|X)
$$
we can minimize EPE pointwise
$$
\hat{G}(x) = \text{argmin}_{g \in \mathcal{G}} \sum_{k=1}^{K} L(\mathcal{G}_k, g) \text{Pr}(\mathcal{G}_k | X = x).
$$
