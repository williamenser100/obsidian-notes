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
u(x)=\underset{\sim}{N} \cdot \underset{\sim}{d_{e}} = [1-\xi, \xi]\b


$$


