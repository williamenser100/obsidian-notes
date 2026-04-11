## Matrismekanik
Vi antar $N$-dimensionellt med en given ON-bas $\ket{\psi_{n}} = \ket{n}$. Vi kan då representera vektorer som koordinatmatriser
$$
\ket{\Psi} = \sum_{n=1}^N c_{n} \ket{n} \implies \bra{\Psi} = (c_{1}^* , \dots, c_{N}^*), \quad \ket{n} = \begin{pmatrix}
c_{1} \\ \vdots \\ c_{N}
\end{pmatrix}   
$$
Operatorer representeras av $N \times N$ matriser:
$$
\hat{A} = \sum_{mn} \ket{m} \langle m | \hat{A} | n \rangle \bra{n} = \sum_{mn} A_{mn}\ket{m} \bra{n}. 
$$
$$
\hat{A} =
\begin{pmatrix}
A_{11} & A_{12} & \cdots \\
A_{21} & A_{22} & \\
\vdots &        & \ddots \\
       &        & A_{NN}
\end{pmatrix}
$$
Observabler representeras av Hermitska operatorer som ger Hermitska matriser:
$$
A_{mn} = \langle m | \hat{A} | n \rangle = \langle \hat{A}m | n \rangle=\langle m | \hat{A}n \rangle = A_{mn}^*.
$$
I basen av sina egenvektorer blir matrisrepresentationen av operatorn:
$$
A_{mn} = \langle m | \hat{A} | n \rangle = a_{n}\langle m | n \rangle = a_{n} \delta_{mn}.
$$
Alltså en diagonalmatris.

## Kvantiserat vs kontinuerligt spektrum
Observabler kan vara kvantiserade eller kontinuerliga, kommer ge ändlig och kontinuerlig bas för Hilbertrummet. Positionsobservabeln $x$ är ett exempel som ger en kontinuerlig. I kontinuerligt fall byts $\ket{n}$ mot $\ket{x}$ och $\sum_{n}$ mot $\int dx$:
$$
1 = \langle \Psi | \Psi \rangle = \int \langle \Psi | x \rangle \langle x | \Psi \rangle dx \quad \text{och} \quad \hat{I} = \int \ket{x} \bra{x} dx.
$$
där $\langle \Psi | x \rangle \langle x | \Psi \rangle = |\langle x | \Psi \rangle|^2$ är sannolikheten att hitta positionen inom $dx$. Vi kan då identifiera att
$$
\Psi(x) = \langle x | \Psi \rangle.
$$
I kvantiserade fallet blir ON-relationen $\langle m | n \rangle = \delta_{mn}$ som i kontinuerliga fallet byts mot
$$
\langle x | x' \rangle = \delta(x-x').
$$
## Delta funktionsnormering
Vi vill normera plana vågorna $=$ rörelsemängdsegenfunktionerna 
$$
\langle x | p \rangle = \Psi_{p}(x) = Ae^{i px/\hbar}
$$
s.a 
$$
\langle p | p' \rangle = \delta(p-p').
$$
Görs med Fouriertransform
$$
\Psi(x) = \frac{1}{\sqrt{ 2\pi }} \int_{-\infty}^{\infty} e^{ikx} \Psi(k) \, dk = \int_{-\infty}^{\infty} \left[ \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{ik(x-y)} \, dk  \right]\Psi(y) \, dy  = \int_{-\infty}^{\infty} \delta(x-y)\Psi(y) \, dy  
$$
alltså kan vi skriva 
$$
\delta(x) = \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{\pm ikx} \, dk, \quad  \delta(k) = \frac{1}{2\pi} \int_{-\infty}^{\infty} e^{\pm ikx} \, dx
$$
ger 
$$
\langle p | p' \rangle = \int_{-\infty}^{\infty} \langle p | x \rangle \langle x | p' \rangle  \, dx = |A|^2 \int_{-\infty}^{\infty} e^{i(p-p')x/\hbar} \, dx = |A|^22\pi \hbar \delta(p-p').
$$
Alltså får vi deltafunktionsnormeringen till
$$
\Psi_p(x) = \langle x | p \rangle = \frac{1}{\sqrt{ 2\pi \hbar }}e^{i p x/\hbar}.
$$
## Gemensamma egenfunktioner
Sats: Två Hermitska operatorer $A,B$ med ickedegenererade egenevärden har samma egenvärden om och endast om de kommuterar. $[A,B] = AB-AB=0$.
## Allmänna osäkerhetsrelationen 
$$
\Delta A \Delta B \ge \frac{1}{2} |\langle [A,B] \rangle|
$$
Om $[A,B]=0$ så är $A$ och $B$ kompatibla och $A$ och $B$ kan var samtidigt bestämda i ett gemensamt egentillstånd. 
Om $[A,B] \ne 0$ så är $A$ och $B$ inkompatibla och $A$ och $B$ kan inte var samtidigt bestämda.
Energins osäkerhet 
$$
\Delta x\Delta E \ge \frac{\hbar}{2m}|\langle p \rangle|
$$

