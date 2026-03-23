## Hilbertrummet
Superpositionsprincipen samt linjäriteten för SE ger att vågfunktionerna bildar Hilbertrummet.
$$
\Psi = \sum_{n} c_{n} \psi_{n}
$$
Vi kallar $\Psi$ för ketvektorer $\ket{\Psi}$  m.a.p en bas i Hilbertrummet. Definiera inre produkten av två vektorer
$$
\langle \Psi_{1} | \Psi_{2} \rangle = \int_{-\infty}^{\infty} \Psi_{1}^* \Psi_{2} \, dx = \langle \Psi_{2} | \Psi_{1} \rangle^*
$$
samt normen $||\Psi||^2=\sqrt{\langle \Psi  | \Psi \rangle}$. $\bra{\Psi}$ kallas dual vektor eller bravektor.

>[!Postulat 1]
> Tillståndet hos ett system är normerade vektorer $\ket{\Psi}$ i Hilbertrummet. Innehåller all information om tillståndet.

## Hermitska operatorer (q-nummer)
Är funktioner som avbildar vektorer på nya vektorer. Har formen
$$
\hat{A}=\ket{\Psi_{1}} \bra{\Psi_{2}}
$$
som avbildar vektorer på ket vektorn $\ket{\Psi_{1}}$. Vi skriver $\hat{A}\ket{\Psi}=\ket{\hat{A}\Psi}$ samt duala bravektor $\bra{\hat{A}\Psi}$.
Definition: Operatorn $\hat{A}$ är Hermitsk om 
$$
\langle \Psi_{1} | \hat{A} \Psi_{2} \rangle = \langle \hat{A} \Psi_{1} | \Psi_{2} \rangle.
$$
Definition: Den adjungerade operatorn $\hat{A}^{\dagger}$ uppfyller
$$
\langle \hat{A}^{\dagger}\Psi_{1} | \Psi_{2} \rangle = \langle \Psi_{1} | \hat{A}\Psi_{2} \rangle.
$$
dvs Hermitsk $\hat{A}^{\dagger}=\hat{A}$.
Skrivsätt för Hermitska operatorer: $\langle \Psi_{1} |\hat{A}| \Psi_{2} \rangle =\langle \Psi_{1} |\hat{A} \Psi_{2} \rangle=\langle \hat{A} \Psi_{1}| \Psi_{2} \rangle$.

Sats: För egenvärdesproblemet $\hat{A}\ket{\Psi_{n}} = a_{n}\ket{\Psi_{n}}$ för Hermitska operatorer gäller
1. $a_{n}$ är reella
2. Egenfunktioner $\ket{\Psi_{n}}, \ket{\Psi_{m}}$ till olika egenvärden är ortogonala. Degeneration om flera egenvektorer till samma egenvärden. Vid degeneration kan vi välja så att vektorerna blir ortogonala.
3. Egenvektorerna utgör en bas för Hilbertrummet. $\ket{\Psi}=\sum_{n}c_{n}\ket{\Psi_{n}}$. 

>[!Postulat 2]
>Observabler representeras av Hermitska operatorer med fullständiga egenvektorer = bildar bas.
>- Postion $x$ : $\hat{x}=x$.
>- Rörelsemängd $p$ : $\hat{p}=\frac{\hbar}{i}\frac{ \partial }{ \partial x }$.
>- Observabel med klassiska utryck: $A(x,p)$ : $\hat{A}=A(\hat{x},\hat{p})$.











