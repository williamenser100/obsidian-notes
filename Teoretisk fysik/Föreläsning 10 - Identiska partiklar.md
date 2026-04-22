**Klassiskt** är alla partiklar särskiljbrar genom att följa exakta banor.
**Kvantmekaniskt** finns inga klassiska banor. Kan inte särskilja identiska partiklar på korta avstånd; då vågfunktionerna överlappar.
## Tvåpartikelsystem
$$
\Psi(\mathbf{r}_{1},\mathbf{r}_{2},t)
$$
uppfyller SE
$$
H\Psi = i\hbar \frac{ \partial \Psi }{ \partial t } 
$$
där 
$$
H = -\frac{\hbar^2}{2m_1} \nabla_1^2 - \frac{\hbar^2}{2m_2} \nabla_2^2 + V(\mathbf{r}_1, \mathbf{r}_2)
$$
## Särskiljbara partiklar
Första exciterade tillståndet
$$
\Psi(x) = a\Psi_{1}(x)\Psi_{0}(x)+b\Psi_{0}(x)\Psi_{1}(x)
$$
$$
\langle \Psi | (x_{1})-x_{2} )^2| \Psi \rangle = \cdots - 2\mathrm{Re}(a^*b+b^*a) \langle \Psi_{1} | x | \Psi_{0} \rangle\langle \psi_{1} | x | \Psi_{0} \rangle
$$
För att KM ska ge entydiga väntevärden måste $a,b$ fixeras. Visa att $b=\pm a$
$$
\psi_{n1}(x)\psi_{n2}(x) = \ket{n_{1}n_{2}} = \ket{\psi_{1}}\otimes \ket{\psi_{2}} 
$$
Definierar utbytesoperatorn
$$
P_{12} \ket{n_{1}n_{2}} =\ket{n_{2}n_{1}} = e^{i\delta}\ket{n_{1}n_{2}} 
$$
$$
P_{12}^2 \ket{n_{1}n_{2}} = P_{12} e^{i\delta} \ket{n_{1}n_{2}} =e^{i 2\delta}\ket{n_{1}n_{2}} =\ket{n_{1}n_{2}} \implies b=\pm a
$$
Nytt postulat i icke-relativistisk KM
>[!Symmetriseringspostulatet]
>Det finns bara två sorters partiklar. **Bosoner** : heltaligt spinn, symmetriska tillstånd under utbyte $\ket{n_{1}n_{2}}=\ket{n_{2}n_{1}}$.  **Fermioner** : halvtaliga spinn, antisymmetriska tillstånd, $\ket{n_{1}n_{2}}=-\ket{n_{2}n_{1}}$.

Två tillåtna tillstånd:
- $\Psi(r_{1},r_{2})=-\Psi(r_{2},r_{1})$ $\implies \chi$ symmetrisk dvs tripletten $\ket{11} = \uparrow \uparrow$, $\ket{10} = \frac{1}{\sqrt{ 2 }}(\uparrow \downarrow + \downarrow \uparrow)$, $\ket{1,-1}=\downarrow\downarrow$.
-  $\Psi(r_{1},r_{2})=+\Psi(r_{2},r_{1})$ $\implies \chi$ antisymetrisk : singletten $\ket{00} = \frac{1}{\sqrt{ 2 }}(\uparrow \downarrow + \downarrow \uparrow)$. 

**Pauliprincipen** : två identiska fermioner kan inte vara i samma tillstånd. 
$$
\psi(r_1, r_2) = A \left[ \psi_a(r_1)\psi_a(r_2) - \psi_a(r_2)\psi_a(r_1) \right] = 0
$$

