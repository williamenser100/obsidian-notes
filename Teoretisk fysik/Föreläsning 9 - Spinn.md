## Spinn
Nytt intrinsiskt (inte pga banrörelse) rörelsemängdsmoment som är **halvtaligt**. 
Stern-Gerlach: silversulfid $Ag_{2}S$, 
Stråle $Ag$-atomer : magnetiskt moment från yttersta elektronen
$$
V = -\boldsymbol{\mu} \cdot \mathbf{B} \implies F_{z} = -\frac{ \partial V }{ \partial z }  = \mu \frac{ \partial B }{ \partial z } \propto S_{z} = \pm \frac{\hbar}{2}. 
$$
SG såg **elektronspin**.
**Nytt postulat** i ickerelativistisk kvantmekanik: (automatisk följd i relavtivistisk KM)
>[!Postulat] 
>Partiklar har intrinsiskt rörelsemängdsmoment : spinn.

$$
\mathbf{S} = (S_{x},S_{y}, S_{y}), \quad \mathbf{S}^2 = S_{x}^2 + S_{y}^2 + S_{z}^2
$$
$$
[S_{x},S_{y}] = i\hbar S_{z}, \quad [S^2, S_{z}] = 0
$$
Spinntillstånd: spinorer $\ket{\chi}$
Egenvektorer
$$
\hat{S}\ket{sm} = s(s+1)\hbar^2\ket{sm}, \quad \hat{S}_{z}\ket{sm} = m\hbar \ket{sm}. 
$$
Hilbertrummet : spinnrummet, totalt tillstånd:
$$
\ket{\Psi} \otimes \ket{\chi}  
$$
Experiment : varje partikel har ett fixt värde på spinnkvanttalet $s$.
- Materiapartiklar : elektroner, protoner, neutroner, kvark : $s=\frac{1}{2}$
- Kraftpartiklar : foton, gluon, $Z$- och $W$-bosoner : $s=1$
- Higgspartikeln : $s=0$
- Gravitonen : $s=2$
## Spinn $\frac{1}{2}$, elektron, proton, neutron
$$
s= \frac{1}{2} \implies m= \pm \frac{1}{2} \implies S_{z} = m\hbar = \pm \frac{\hbar}{2}.
$$
$$
S^2 = s(s+1) \hbar^2 = \frac{3\hbar^2}{4}
$$
$$
S_{z} = + \frac{\hbar}{2} \text{ spinn upp} : \ket{\frac{1}{2},+ \frac{1}{2}} = \uparrow = \chi_{+} = \begin{pmatrix}
1 \\
0
\end{pmatrix} = \ket{+}  = \ket{0} 
$$
$$
S_{z} = - \frac{\hbar}{2} \text{ spinn ner} : \ket{\frac{1}{2}, -\frac{1}{2}} = \downarrow = \chi_{-} =\begin{pmatrix}
0 \\
1
\end{pmatrix} = \ket{-} =\ket{1} 
$$
Spinnrummet är tvådimensionellt fullständigt Hilbertrum med bas $\chi_{+},\chi_{-}$

Fullständighet : identtietsoperatorn $\hat{I}\ket{\psi}=\ket{\psi}\ \ \forall \ket{\psi}$
$$
\hat{I} = \sum_{s=1/2,m=\pm 1/2} \ket{sm} \bra{sm}  = \ket{+} \bra{+} + \ket{-} \bra{-} = \begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}
$$
Spinnoperatorerna för $\hat{S}^2, \hat{S}_{z}$ är diagonala med egenvärdena $=$ mätvärdena som diagonal.
$$
\hat{S}^2 = \frac{3}{4}\hbar^2 \begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}
$$
$$
\hat{S}_{z} = \frac{\hbar}{2}\begin{bmatrix}
1 & 0 \\
0 & -1
\end{bmatrix}
$$
Stegoperatorer definieras av 
$$
S_{\pm} = S_{x} \pm iS_{y} 
$$
Kommer då ge 
$$
S_{+} = \hbar \begin{bmatrix}
0 & 1 \\
0 & 0
\end{bmatrix}
\quad 
S_{-} = \hbar \begin{bmatrix}
0 & 0 \\
1 & 0
\end{bmatrix}
\implies
$$
$$
S_x = \frac{1}{2}(S_+ + S_-) = \frac{\hbar}{2}
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix},
\quad
S_y = \frac{1}{2i}(S_+ - S_-) = \frac{\hbar}{2}
\begin{pmatrix}
0 & -i \\
i & 0
\end{pmatrix}
$$
Pauli spinnmatriser:
$$
\sigma_x =
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix},
\quad
\sigma_y =
\begin{pmatrix}
0 & -i \\
i & 0
\end{pmatrix},
\quad
\sigma_z =
\begin{pmatrix}
1 & 0 \\
0 & -1
\end{pmatrix}
$$
Allmänn spinor:
$$
\ket{\chi} = a\ket{\chi_{+}} +b\ket{\chi_{-}}  = \begin{bmatrix}
a \\
b
\end{bmatrix}
$$
Normering:
$$
\langle \chi | \chi \rangle = (a^*, b^*)\begin{pmatrix}
a \\
b
\end{pmatrix}
= |a|^2 +|b|^2 = 1
$$
Egenvektorer till $\hat{S}_{x},\hat{S}_{y}$ :
$$
\hat{S}_{x}\chi_{\pm}^x = \pm \frac{\hbar}{2} \chi_{+}^x, \quad\chi_{\pm}^x = \frac{1}{\sqrt{ 2 }} \begin{pmatrix}
1 \\
\pm 1
\end{pmatrix}
\quad
\hat{S}_{y}\chi_{\pm}^y = \pm \frac{\hbar}{2} \chi_{+}^y, \quad\chi_{\pm}^y = \frac{1}{\sqrt{ 2 }} \begin{pmatrix}
1 \\
\pm i
\end{pmatrix}
$$

$$
\hat{S}_{x}\uparrow = \frac{\hbar}{2} \downarrow, \quad \hat{S}_{x}\downarrow = \frac{\hbar}{2} \uparrow
$$
$$
\hat{S}_{y}\uparrow = i\frac{\hbar}{2} \downarrow, \quad \hat{S}_{x}\downarrow = i\frac{\hbar}{2} \uparrow
$$
## Pålagt magnetfält
$$
\boldsymbol{\mu} = \frac{gq}{2m}\mathbf{S}
$$
$g$ är konstant ur experiment, olika för olika partiklar. $q$ elektriskt laddning.
$$
H = V = -\boldsymbol{\mu} \cdot \mathbf{B} = -\frac{gq}{2m} \mathbf{B} \cdot \mathbf{S}
$$
Välj 
$$
\mathbf{B} = (0,0,B) \implies H=-\frac{gqB}{2m}S_{z}.
$$
**Elektron**:
 $$
g= 2.00\dots,  \quad q = -e,\quad \boldsymbol{\mu} = -\frac{e}{m}\mathbf{S}, \quad\mu_{z} = -\frac{e}{m}S_{z} = \mp \frac{e\hbar}{2m}
$$
$$
\mu_{B} = \frac{e\hbar}{2m} \text{ Bohrmagnetonen}
$$
**Proton**:
$$
g=5.58, \quad q = \pm e, \quad \mu = \frac{q}{2m} S_{z} = \pm \mu_{p} 
$$
**Neutron**:














