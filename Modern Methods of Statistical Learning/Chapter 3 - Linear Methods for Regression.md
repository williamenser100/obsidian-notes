Linear regression model assumes the regression function $E(Y|X)$ is linear in the inputs $X_{1},\dots,X_{P}$. The linear regression model has the form
$$
f(X) = \beta_{0}+\sum_{j=1}^p X_{j} \beta_{j}
$$
## The Gauss-Markov Theorem
We want to estimate $\theta=a^T\beta$, for example $f(x_{0})=x_{0}^T\beta$ are on this form. Its least square estimate 
$$
\hat{\theta}=a^T\hat{\beta}=a^T(X^TX)^{-1}X^T\mathbf{y}.
$$
which is a linear function $\mathbf{c}_{0}^T\mathbf{y}$ of the response vector $\mathbf{y}$. This means that if the linear model is correct, then 
$$
E(a^T\hat{\beta}) = E(a^T(\mathbf{X}^T\mathbf{X})^{-1}\mathbf{X}^T\mathbf{y}) = a^T(\mathbf{X}^T\mathbf{X})^{-1}\mathbf{X}^T\mathbf{X}\beta = a^T\beta.
$$
which means that $a^T\hat{\beta}$ is unbiased. (assumed linear model means $Y=X\beta$, the rest of the above expression is constant for fixed $X$). 
The Gauss-Markov Theorem states:
If there are any other linear estimators $\tilde{\theta}=\mathbf{c}^T\mathbf{y}$ that is unbiased for $a^T\beta$, then
$$
\text{Var}(a^T\hat{\beta}) \le \text{Var}(\mathbf{C}^T\mathbf{y}).
$$
The mean squared error of an estimator $\tilde{\theta}$ estimating $\theta$:
$$
\text{MSE}(\tilde{\theta}) = E(\tilde{\theta}-\theta)^2=\text{Var}(\tilde{\theta})+[E(\tilde{\theta})-\theta]^2.
$$
The first term is the variance and the second term is the bias squared. The GM theorem states that the least square estimator has the smallest MSE for unbiased estimators. But there may as well exist a a biased estimator with smaller mean squared error, which would trade some bias for a smaller variance. When choosing an estimation model, the variance bias relationship needs to be considered.
## Univariate Regression
The univariate regression model
$$
Y=X\beta+\varepsilon
$$
which is the original linear model with $p=1$ and no intercept. Then, the least square estimator and residual is
$$
\hat{\beta}=\frac{\sum_{1}^Nx_{i}y_{i}}{\sum_{1}^Nx_{i^2}}, \quad r_{i}=y_{i} -x_{i}\hat{\beta}. 
$$
which can be written as 
$$
\hat{\beta}=\frac{\langle \mathbf{x} | \mathbf{y} \rangle}{\langle \mathbf{x} | \mathbf{x} \rangle}, \quad \mathbf{r}=\mathbf{y}-\mathbf{x}\hat{\beta}
$$
## Multiple outputs
For multiple outputs $Y_{1},Y_{2},\dots,Y_{K}$ to predict from inputs $X_{0},X_{1},\dots,X_{p}$. Assume linear model
$$
Y_{k}= \beta_{0}k+\sum_{j=1}^p X_{j}\beta_{jk} + \varepsilon_{k}=f_{k}(X)+\varepsilon
$$
which can be written as 
$$
\mathbf{Y}=\mathbf{X}\mathbf{B}+\mathbf{E}
$$
where $\mathbf{Y}$ is the $N\times K$ response matrix with $ik$ entry $y_{ik}$. $\mathbf{X}$ is $N\times p+1$ input matrix, $\mathbf{B}$ is the $p+1\times K$ matrix of parameters and $\mathbf{E}$ is the $N\times K$ matrix of errors. 
This can generalize the univariate loss function with a matrix as the input $RSS(\mathbf{B})$ instead of $RSS(\beta)$ as:
$$
\text{RSS}(\mathbf{B}) = \sum_{k=1}^{K} \sum_{i=1}^{N} (y_{ik} - f_k(x_i))^2 = \text{tr}[(\mathbf{Y} - \mathbf{X}\mathbf{B})^T(\mathbf{Y} - \mathbf{X}\mathbf{B})]
$$
which is on the same form as before
$$
\hat{B} = (X^TX)^{-1} X^TY.
$$
This means that multiple outputs do not affect each others estimates. 

So what about if the errors in the matrix $E$ are correlated? The elements of $E$ are $\varepsilon=(\varepsilon_{1},\dots,\varepsilon_{k})$ and the covariance matrix for $\varepsilon$ is $\Sigma$. Then,
$$
RSS(B;\Sigma) = \sum_{i=1}^N(y_{i}-f(x_{i}))^T\Sigma^{-1}(y_{i}-f(x_{i}))
$$
It can be shown that the solution is still
$$
\hat{B} = (X^TX)^{-1} X^TY.
$$






