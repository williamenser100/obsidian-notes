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


