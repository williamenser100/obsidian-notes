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
Detta kommer ge (till första ordningen)
$$
P_{a\to b} = \frac{|V_{ab}|^2}{\hbar^2} \frac{\sin^2((\omega_{0}-\omega)t/2)}{(\omega_{0}-\omega)^2}
$$
Sannolikheten är störst när frekvensen $\omega$ är nära systemets egna frekvens $\omega_{0}$, vilket är resonans.

För långa $t$ får vi 
$$
c_{b} = \frac{\pi V_{ab}}{i\hbar} \delta(\omega_{0}-\omega)
$$
Definiera övergångshastigheten $R=P_{a\to b}/t$ 
$$
R = \frac{\pi}{2\hbar^2} |V_{ab}|^2 \delta(\omega_{0}-\omega)
$$
Deltafunktionen säger att övergången sker om 
$$
E_{b} = E_{a}-\hbar \omega
$$
Systemet sänker sin energi från $E_{a}$ till $E_{b}$ genom att avge $\hbar \omega$ till omgivningen. x
## Emission och absorption av strålning 
Absorption

Emission

Stimulerad emission

Spontan emission

## Inkoherent störning
Vi antar opolariserad strålning som träffar atomen från alla riktningar
$$
u = \epsilon_{0}E_{0}^2\cos^2\omega t
$$
Denna strålningsenergis (medelvärde) används som störning med $V_{ab}=-DE_{0}$
$$
|V_{ab}|^2=\frac{2D^2}{\epsilon_{0}}u
$$
För många tillämpningar består strålningen av många olika frekvenser istället för en enda frekvens. Vi antar då en fördelning av frekvenser med energitätheten $\rho(\omega)$ per frekvensintervall. $\implies u\to \rho(\omega)d\omega$. Då kommer sannolikheten ges då av summan över alla frekvenser
$$
P_{a\rightarrow b}(t) = \frac{2D^2}{\epsilon_0\hbar^2} \int_0^{\infty} \rho(\omega) \frac{\sin^2((\omega_0 - \omega)t/2)}{(\omega_0 - \omega)^2} d\omega
$$
som approximeras och fås då till
$$
P_{a\to b}(t) = \frac{\pi D^2}{\epsilon_{0} \hbar^2}\rho(\omega_{0})t
$$
Övergångshastigheten $R=\frac{dP}{dt}$ 
$$
R = \frac{\pi D^2}{\epsilon_{0}\hbar^2}\rho(\omega_{0})
$$
Om vi tar hänsyn till att strålningen kommer från alla riktningar så kommer övergångshastigheten bli
$$
R_{a\to b} = \frac{\pi}{3\epsilon_{0}\hbar^2} |D|^2\rho(\omega_{0})
$$
## Einsteins A och B koefficienter
Koefficienten i övergångshastigheten är Einsteins B-koefficient
$$
B_{ab} = \frac{\pi}{3\epsilon_0\hbar^2}|D|^2 = B_{ba}
$$






## Livstiden hos ett exciterat tillstånd


