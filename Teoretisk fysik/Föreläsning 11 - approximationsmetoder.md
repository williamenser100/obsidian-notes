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
## Anharmonisk oscillator


