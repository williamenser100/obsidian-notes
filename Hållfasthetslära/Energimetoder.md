Yttre laster deformerar kroppar, dvs utför arbete $W_{A}$. Betrakta stång fäst i ena änden och belastad i andra med en kraft $P$, $\implies P=\frac{EA}{L}\delta$. Vet att $dW_{A} = Pd\delta$.
$$
W_{A}=\int Pd\delta = \int AL\sigma d\varepsilon=V\underbrace{ \int_{0}^\varepsilon \sigma d\varepsilon }_{ w_{e} }. 
$$
Där vi definierar $W_{A} = Vw_{e}$ elastisk energi/volymsenhet i material. För stång $\sigma=E\varepsilon$ blir 
$$
W=V \frac{E\varepsilon^2}{2}.
$$
Motsvarande i skjuvning:
$$
\tau=G\gamma,\quad \gamma=\frac{u}{h},\quad d\gamma=\frac{du}{h}
$$
$$
W_{e}=\int \underbrace{ \tau b t }_{ \text{kraft} } du = bth \int \tau d\gamma = V\int_{0}^\gamma G \gamma d\gamma = V \frac{1}{2} G \gamma^2.
$$
## Böjning/krökning av balk
$$
\varepsilon=Hz = -w''z, \quad \sigma=E\varepsilon = -Ew''z.
$$
Då blir 
$$
W_{e}=\int w_{e}dV = \int_{0}^L \left[ \frac{1}{2} \int_{A}E(w'')^2z^2dA \right]dx = \frac{1}{2}\int EI (w'')^2dx.
$$
## Vridning av axel
$$
\gamma = \frac{\theta}{l}r = \frac{d\theta}{dx}r, \quad \tau =G \gamma = G\theta'r.
$$
Då blir 
$$
W_{e}=\int_{V}w_{e}dV = \{\dots\} = \int_{0}^LGK(\theta')^2dx
$$
där 
$$
K=\int_{r_{i}}^{r_{y}} 2\pi r^3dr.
$$

## Virtuella arbetets princip
För en 1D stång med variation längs med gäller 
$$
\frac{d}{dx}\left( EA \frac{du}{dx} \right) + K_{x} A = 0
$$
med R.V
$$
u(x=0)=0, \quad EA \frac{du}{dx} \Bigg|_{x=L} = P.
$$
Om vi betraktar $W_{e}$ med en störning $\delta u$ som ett variationsproblem får vi resultatet 
$$
\delta U=0.
$$
Vilket är virtuella arbetets princip (VAP).

## Potentiella energins minimum
Potentiella energin $U$ är 
$$
U= W_{e} - \text{potential av alla yttre laster}.
$$
Alltså säger VAP att $U$ har ett extremvärde/minimum och att 
$$
\delta U=0
$$
motsvarar att diffekvationen och R.V är strikt uppfyllda.
Vilket är potentiella energins minimum (PEM).

