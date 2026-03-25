## Finita elementmetoden
Approximativ lösning av fältproblem. Söker fält $u(x)$ där 
$$
W_{e}=\frac{1}{2}\int EA \left( \frac{du}{dx} \right)^2dx.
$$
Delar upp så att integraler beaktas styckvis i s.k element ($e$), där ändpunkter utgör noder ($k$), vars förskjutning $u_{k}$ är nod/element frihetsgrader DOFs $\underset{\sim}{d_{e}}$ som är sökta obekanta, där fältet representeras approximativt, dvs en ansats mha DOF $\underset{\sim}{d_{e}}$. Görs med hjälp av s.k
Formfunktioner $\underset{\sim}{N}=[N_{1(x)},N_{2}(x)]$, så att 
$$
u(x)=\underset{\sim}{N_{1}} \cdot\underset{\sim}{d_{e}}=N_{1}\cdot u_{k}+N_{2}\cdot u_{k+1}
$$
i varje element.
Ex: Ett linjärt element
$$
u(x)=\underset{\sim}{N} \cdot \underset{\sim}{d_{e}} = [1-\xi, \xi]\begin{bmatrix}
u_{1} \\ u_{2}
\end{bmatrix}
$$
$$
\varepsilon(x)=\frac{du}{dx}=\frac{1}{l_{e}} \frac{du}{d\xi}=\frac{1}{l_{e}} \frac{d}{d\xi} \underset{\sim}{N} \underset{\sim}{d_{e}} = \underbrace{ \frac{1}{l_{e}}[-1,1] }_{ \underset{\sim}{B} } \underbrace{ \begin{bmatrix}
u_{1} \\u_{2}
\end{bmatrix} }_{ \underset{\sim}{d_{e}} }
$$
Potentiell energi:
$$
U=\frac{1}{2} \int \underset{\sim}{d_{e}}^T\cdot\underset{\sim}{B}^T EA \ \underset{\sim}{B}\cdot \underset{\sim}{d_{e}} dx - \int K_{x}\underset{\sim}{d_{e}}^T \cdot \underset{\sim}{N}^T A dx - \sum P_{j}\underset{\sim}{d_{e}}^T \underset{\sim}{N}(x_{j})
$$
Skrivs som
$$
U=\frac{1}{2}\underset{\sim}{d_{e}}^T \cdot K\cdot \underset{\sim}{d_{e}} - \underset{\sim}{d_{e}}^T \cdot \underset{\sim}{F}.
$$
Nu, VAP/PEM ges av
$$
\frac{ \partial U }{ \partial d } = u 
$$
FEM-ekvation:
$$
\underset{\sim}{K}\cdot \underset{\sim}{d_{e}}=\underset{\sim}{F}.
$$
Sen assemblera (många) element till hela strukturen $\implies$ lös.


