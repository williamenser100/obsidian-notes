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
