## Hilbertrummet
Superpositionsprincipen samt linjäriteten för SE ger att vågfunktionerna bildar Hilbertrummet.
$$
\Psi = \sum_{n} c_{n} \psi_{n}
$$
^superpositionsprincipen
Vi kallar $\Psi$ för ketvektorer $\ket{\Psi}$  m.a.p en bas i Hilbertrummet. Definiera inre produkten av två vektorer
$$
\langle \Psi_{1} | \Psi_{2} \rangle = \int_{-\infty}^{\infty} \Psi_{1}^* \Psi_{2} \, dx = \langle \Psi_{2} | \Psi_{1} \rangle^*
$$
^Inre-produkt-hilbertrum
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
^Hermitesk-operator
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

Att operatorerna är Hermitska visas enkelt med partiell integration i $\langle \Psi_{1} | \hat{x} | \Psi_{2} \rangle$ samt $\langle \Psi_{1} | \hat{p} | \Psi_{2} \rangle$ under antagandet $\Psi \to 0$ då $x \to \infty$.
## Fullständighet
ON-bas $\ket{\Psi_{n}}=\ket{n}$ (beteckning). Alltså kan vi för varje $\ket{\Psi}$ skriva
$$
\ket{\Psi} =\sum_{n}c_{n}\ket{\Psi_{n}}= \sum_{n}c_{n}\ket{n}.
$$
Koefficienten $c_{n}$ ges av
$$
\langle n | \Psi \rangle = \sum_{n} c_{n} \underbrace{\langle n | m \rangle}_{=\delta_{mn}} = c_{n} \implies \ket{\Psi} =\sum_{n} \ket{n} \langle n | \Psi \rangle.
$$
Där vi infört projektionsoperatorn $\hat{p}=\ket{n}\bra{n}$, identitetsoperatorn ges som fullständighetsrelationen
$$
\hat{I}=\sum_{n}\ket{n}\bra{n}
$$
Som vi kan använda för att: 
Skriva operator i basen: 
$$
\hat{A} = \hat{I}\hat{A}\hat{I} = \sum_{m,n} \ket{m} \langle m | \hat{A} | n \rangle \bra{n} =\sum_{m,n} = A_{mn} \ket{m} \bra{n} 
$$
Norm av vektor
$$
\langle \Psi | \Psi \rangle = \langle \Psi | \hat{I} | \Psi \rangle = \sum_{n} \langle \Psi | n \rangle\langle n | \Psi \rangle = \sum_{n}|c_{n}|^2 = 1
$$
m.m

>[!Postulat 3]
>Resultatet av en mätning av en observabel $A$ i tillståndet $\ket{\Psi}$ är ett slumpmässigt egenvärde $a_{n}$ till $\hat{A}$ som fås med sannolikhet $|c_{n}|^2=|\langle\Psi_{n}  | \Psi \rangle|$ där . Mätningar ändrar systemets tillstånd till motsvarande egentillstånd $\ket{\Psi}\to \ket{\Psi_{n}}$, vilket kallas att tillståndet kollappsar eller reduceras.

En observabel är antingen bestämd eller osäker:
- Om tillståndet är ett egentillstånd till en observabel $A$, t.ex $\ket{\Psi}=1$ med egenvärde $a_{1}$, så ger en mätning av $A$ svaret $a_{1}$ med sannolikhete $|c_{n}|^2=1$ och $A$ kallas bestämd.
- I superposition med ickedegenererade egenvärden t.ex $\ket{\Psi}=c_{1}\ket{1} + x_{2}\ket{2}$ med $a_{1} \neq a_{2}$ är inte ett egentillstånd och observabeln blir därför osäker. En mätning av $A$ ger svaret $a_{1}$ med sannolikhet $|c_1|^2$ och $a_{2}$ med sannolikhet $|c_{2}|^2$.

>[!Postulat 4]
>Tillståndsvektorn $\ket{\Psi(t)}$ uppfyller SE: $\hat{H}\ket{\Psi(t)}=i\hbar \frac{d}{dt} \ket{\Psi(t)}$.

Betyder att tidsutvecklingen är deterministiskt, så länge mätningar inte görs.







