Finns problem som ej kan lösas numeriskt, men som kan approximeras
## Störningsteori - ickedegenererade fallet
Vill hitta lösningar till
$$
H\psi_{n} = (H^0 +V)\psi_{n} = E_{n}\psi_{n}
$$
mha det ostörda problemet som antas ha känd lösning
$$
H^0 \psi_{n}^0 = E_{n}^0 \psi_{n}^0
$$
med ickedegenererade egenvärden. 
Vi approximerar med ostörda lösningen
$$
E_n = \langle \psi_n | H | \psi_n \rangle 
\approx \langle \psi_n^0 | H | \psi_n^0 \rangle 
= E_n^0 + \langle \psi_n^0 | V | \psi_n^0 \rangle
$$
Bilda $H = H^0 +\lambda V$, sök lösningar som potensserie i $\lambda$
$$
\begin{align}
\psi_n &= \psi_n^0 + \lambda \psi_n^1 + \lambda^2 \psi_n^2 + \cdots \\
E_n &= E_n^0 + \lambda E_n^1 + \lambda^2 E_n^2 + \cdots
\end{align}
$$
ger
$$
\begin{align}
\text{nollte ordningen:} \quad & H^0 \psi_n^0 = E_n^0 \psi_n^0 \\
\text{första ordningen:} \quad & H^0 \psi_n^1 + V \psi_n^0 = E_n^0 \psi_n^1 + E_n^1 \psi_n^0 \\
\text{andra ordningen:} \quad & H^0 \psi_n^2 + V \psi_n^1 = E_n^0 \psi_n^2 + E_n^1 \psi_n^1 + E_n^2 \psi_n^0
\end{align}
$$
Om vi bildar inre produkten av första ordningens termer får vi **första ordningens korrektion till energiegenvärdena** 
$$
E_{n}^1 =\langle \psi_{n}^0 | V | \psi_{n}^0 \rangle
$$
Om vi utvecklar första ordningen korrektion i de ostörda basfunktionerna
$$
\psi_{n}^1 = \sum_{m\ne n} c_{m} \psi_{m}^0, \quad c_{m} = \langle\psi_{m}^0  | \psi_{n}^1 \rangle
$$
vilket kommer ge **första ordningens korrektion till tillståndet**
$$
\psi_n^1 = \sum_{m \ne n} \frac{\langle \psi_m^0 \mid V \mid \psi_n^0 \rangle}{E_n^0 - E_m^0} \, \psi_m^0
$$
För **andra ordningens korrektion till energin** fås
$$
E_n^2 = \sum_{m \ne n} \frac{\left| \langle \psi_m^0 \mid V \mid \psi_n^0 \rangle \right|^2}{E_n^0 - E_m^0}
$$
## Anharmonisk oscillator exempel
$$
H^0 = \frac{p^2}{2m} + \frac{1}{2} m \omega^2 x^2, 
\quad 
V = \lambda \frac{m^2 \omega^3}{\hbar} x^4, 
\quad 
E_n^1 = \lambda \frac{m^2 \omega^3}{\hbar} \langle n \mid x^4 \mid n \rangle
$$
$$
x = \sqrt{\frac{\hbar}{2m\omega}} (a^\dagger + a)
\;\Rightarrow\;
x^4 = \left( \frac{\hbar}{2m\omega} \right)^2 (a^\dagger + a)^4
$$

som efter jobb kommer ge
$$
\langle n \mid (a^\dagger + a)^4 \mid n \rangle = 6n^2 + 6n + 3 = 3(2n^2 + 2n + 1)
$$
alltså
$$
\langle E_n^1 \rangle 
= \lambda \frac{m^2 \omega^3}{\hbar} \left( \frac{\hbar}{2m\omega} \right)^2 3(2n^2 + 2n + 1)
= \frac{3\lambda}{4} \hbar \omega (2n^2 + 2n + 1)
$$
## Elektronens anomala magnetiska moment

## Degenererad störningsräkning
Vid degenererade ostörda energier fungerar inte ovan
Tvåfalt degenererad nivå
$$
H^0 \psi_a^0 = E^0 \psi_a^0, \quad
H^0 \psi_b^0 = E^0 \psi_b^0, \quad
\langle \psi_a^0 \mid \psi_b^0 \rangle = 0
$$
söker
$$
\psi = \psi^0 + \psi^1 = \alpha\psi_{a}^0 + \beta\psi_{b}^0 +\psi^1
$$
Första ordningens korrektion blir
$$
H^0 \psi^1 + V \psi^0 = E^0 \psi^1 + E^1 \psi^0
$$
som med inre produkten med $\psi_{a}^0$ ger
$$
\alpha W_{aa} + \beta W_{bb} = \alpha E^1
$$
där 
$$
W_{ij} \equiv \langle \psi_{i}^0 | V | \psi_{j}^0 \rangle, \quad i,j = a,b
$$
som kommer ge ekvationssystemet
$$
\begin{pmatrix}
W_{aa}  & W_{ab} \\
W_{ba}  & W_{bb}
\end{pmatrix} \begin{pmatrix}
\alpha \\
\beta
\end{pmatrix} = E^1
\begin{pmatrix}
\alpha \\
\beta
\end{pmatrix}
$$
Vi vill välja ostörda basfunktioner som diagonaliserar störningen s.a $W_{ab} =W_{ba}=0$. Då blir
$$
E_+^{1} = W_{aa} = \langle \psi_a^{0} \mid V \mid \psi_a^{0} \rangle, 
\quad
E_-^{1} = W_{bb} = \langle \psi_b^{0} \mid V \mid \psi_b^{0} \rangle
$$
Om detta inte fungerar behöver vi diagonalisera, då fås
$$
E_{\pm}^{1} = \frac{1}{2} \left( W_{aa} + W_{bb} \pm \sqrt{(W_{aa} - W_{bb})^2 + 4|W_{ab}|^2} \right)
$$
## Variationsmetoden
Bygger på idén att införa en variationsvågfunktion $\psi(\lambda)$ som beror på variationsparameter $\lambda$. Grundtillståndsenergin uppskattas enligt
$$
E_{0} \approx \langle \psi(\lambda) | H | \psi(\lambda) \rangle
$$
Sats: För vilken vågfunktion som helst gäller
$$
E_{0} \le \langle \psi | H | \psi \rangle
$$
