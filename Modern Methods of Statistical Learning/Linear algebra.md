If $\varepsilon$ is the error vector for every observation $Y_{i}$
$$
\varepsilon = \begin{pmatrix} \varepsilon_1 \\ \varepsilon_2 \\ \vdots \\ \varepsilon_N \end{pmatrix}, \qquad \varepsilon_i = Y_i - (\beta_0 + \sum_j x_{ij} \beta_j).
$$
then, if $\varepsilon \sim N(\mathbf{\mu}, \mathbf{\Sigma})$ and $\mathbf{A}$ is a constant matrix, then 
$$
\mathbf{A}\varepsilon \sim N(\mathbf{A}\mathbf{\mu}, \mathbf{A}\mathbf{\Sigma}\mathbf{A}^T)
$$
