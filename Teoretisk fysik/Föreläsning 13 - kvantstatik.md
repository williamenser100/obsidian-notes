## Plancks strålningslag
Svartkroppsstrålning/elektromagnetisk strålning inuti en kavitet $V=L^3$. Vill bestämma energi per volymstäthet $u=E/V$. 
$$
\frac{du}{d\omega} =\frac{1}{V} g(\omega)\langle E \rangle
$$
där $g(\omega)$ är antalet tillstånd per frekvensintervall. Visar sig att
$$
g(\omega) = V \frac{\omega^2}{\pi^2c^3}
$$
Det visar sig att klassiska fysiken inte fungerar vid stora frekvenser vilket motsvarar korta våglängder. Totala energin divergerar. $\implies$ Vi måste räkna kvantmekaniskt.
Postulera att strålningsenergin kvantiseras $E=n\hbar \omega, n=0,1,2,\dots$ Medelenergin:
$$
\langle E  \rangle = \langle  n  \rangle \hbar \omega = \frac{1}{Z} \sum_{n} E e^{-\beta E} = \frac{\hbar \omega}{e^{\beta \hbar \omega}-1}
$$
Medelantalet fotoner med energi $\hbar \omega$ s.k Bose-Einsteinfördelningen
$$
\langle  n  \rangle = \frac{1}{e^{\beta \hbar \omega}-1}
$$
Planckfördelningen:
$$
\frac{du}{d\omega} = \frac{\hbar \omega^3}{\pi^2c^3} \frac{1}{e^{\beta \hbar \omega}-1}
$$
## Termiska medelvärden
System med $N \sim 10^{23}$ identiska icke växelverkande partiklar. Termiska medelvärden definieras mha medelockupationstalen. T.ex medelockupationstalet $f_{k}$
$$
\langle  E  \rangle = \sum_{n} \langle  n_{k}  \rangle E_{k} = \sum_{n} f_{k} E_{k}
$$
summerar över enpartikeltillstånd $k$, $n_{k}$ är antalet partiklar i enpartikeltillståndet $k$ och $E_{k}$ är energin för en partikel i tillståndet $k$. Medelockjupationstalet kallas fördelningsfunktionen
$$
f_k = \langle n_k \rangle = \frac{\sum_{n_k} n_k e^{-\beta(E_k - \mu)n_k}}{\sum_{n_k} e^{-\beta(E_k - \mu)n_k}}
$$
där $\mu$ är kemiska potentialen som reglerar partikelantalet genom
$$
\langle  N  \rangle = \sum_{n} f_{k}(\mu)
$$
Planckfördelningen har $\mu=0$, materiepartiklar har $\mu=\mu(T)$, tempertaturberoende funktion. 

## Fermi-Dirac och Bose-Einstein fördelningar
Pauliprincipen säger att för identiska fermioner är $n_{k}=0,1$. Fördelningsfunktionen vlir
$$
f_k = \frac{\sum_{n_k=0,1} n_k e^{-\beta(E_k-\mu)n_k}}{\sum_{n_k=0,1} e^{-\beta(E_k-\mu)n_k}} = \frac{e^{-\beta(E_k-\mu)}}{1 + e^{-\beta(E_k-\mu)}}
$$
Vilket ger Fermi-Dirac fördelningen
$$
f_{K}^{FD}
$$

