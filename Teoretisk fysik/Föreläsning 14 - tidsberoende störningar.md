## Störningsräkning
$$
H^0\ket{n} = E_{n}^0 \ket{n}  
$$
Vill lösa 
$$
H(t) = H^0 + \lambda V(t)
$$
Problem: Om initialtillståndet är $\ket{a}$ vid $t=t_{0}=0$, vad är sannolikheten att tillståndet vid $t$ är $\ket{b}$?

Eftersom ostörda egentillstånd är fullständiga 
$$
\ket{\Psi(t)} = \sum_{n} c_{n}(t) e^{-iE_{n}t/\hbar}\ket{n}  
$$
där $c_{n}(t)$ kommer från störningen $V(t)$. Initialvärdet ger
$$
c_{n}(0) = \langle n | \Psi(o) \rangle
$$
Om vi sätter in i SE fås 
$$
\frac{dc_b(t)}{dt} = \frac{1}{i\hbar} \sum_n c_n(t) e^{i(E_b - E_n)t/\hbar} \langle b | \lambda V | n \rangle
$$
Genom att ansätta en störningsserie så får vi första ordningens term $c_{b}^1$
$$
c_{b}^1 = \frac{1}{i\hbar} \int_{0}^t e^{i\omega_{0}t'} V_{ba}(t') dt'
$$
där
$$
\omega_{0} \equiv \frac{E_{b}-E_{a}}{\hbar},\quad V_{ba} \equiv \langle b | V | a \rangle
$$
## Konstant störning
En konstant störning slås på under en tid $t$, $V(\mathbf{r},t)=V(\mathbf{r})$. Resultatet blir att sannolikheten oscillerar med tiden
$$
P_{a\to b} = \frac{|V_{ab}|^2}{\hbar^2} \frac{\sin^2(\omega_{0}t/2)}{(\omega_{0}/2)^2}
$$
## Oscillerande störning
Systemets utsätts för ett oscillerande fält som beskrivs som oscillerande störning
$$
V(t) = V(\mathbf{r})\cos \omega t
$$
Detta kommer ge
$$
P_{a\to b} = \frac{|V_{ab}|^2}{\hbar^2} \frac{\sin^2((\omega_{0}-\omega)t/2)}{(\omega_{0}-\omega)^2}
$$
