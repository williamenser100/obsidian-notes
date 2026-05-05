Det ostörda problemet har
$$
H^0 = \frac{p^2}{2m} + V^0 =\frac{p^2}{2m}-\frac{e^2}{4\pi\epsilon_{0}r}
$$
med 
$$
E^0_{100} = -\frac{1}{2} \frac{e^2}{4\pi\epsilon_{0}a}=-13.6 \text{ eV}
$$
där $a$ är Bohrradien. Det ostörda vätetillståndet 
$$
\psi_{100}^0 = \frac{e^{-r/1}}{\sqrt{ \pi a^3 }}
$$
Det $n$:te energinivån har degeneration $2n^2$. $\implies$ Vi behöver degenerarad störningsräkning.
Vi söker en ostörd bas där störningen blir diagonal. Förkorta $E_{n} = E_{nlm}^0$. 
Inför finstrukturkonstanten
$$
\alpha = \frac{e^2}{4\pi\epsilon_{0}\hbar c}\approx \frac{1}{137}
$$

## Relativistisk korrektion
$$
E_n^1 =  -\frac{(E_n)^2}{2mc^2}\left(\frac{4n}{l+1/2} - 3\right)
$$
## Spinn-bankoppling
$$
E_n^1 = \frac{(E_n)^2}{2mc^2}\left(3 - \frac{4n}{j+1/2}\right)
$$
## Zeemaneffekten
Zeeman-störningen är 
$$
V = -(\boldsymbol{\mu}_{l}+\boldsymbol{\mu}_{s})\cdot \mathbf{B}=\frac{e}{2m} \mathbf{B}\cdot(\mathbf{J}+\mathbf{S})
$$
där
$$
J \equiv \mathbf{L}+\mathbf{S}
$$
### Svaga fält $B \ll B_{int}$
Första ordningens energikorrektion blir
$$
E^1 = \mu_{B} gBm_{j}
$$
där $g$ är Landé faktorn
$$
g = 1 + \frac{j(j+1) + s(s+1) - l(l+1)}{2j(j+1)}
$$
och Bohrmagnetonen
$$
\mu_{B} = \frac{e\hbar}{2m}.
$$
### Starka fält $B\gg B_{int}$ : Paschen-Back effekt
Zeemaneffekten dominerar. Första ordningens korrektion blir
$$
E^1 = \mu_{B} B(m_{l}+2m_{s})
$$
Som kommer ge
$$
E^1_{fs} = \frac{13.6 \text{ eV}}{n^3} \alpha^2 \left( \frac{3}{4n} - \frac{l(l+1) - m_l m_s}{l(l+1/2)(l+1)} \right)
$$
## Hyperfinstruktur
Den hyperfina strukturen tar utöver elektronens magnetiska moment också hänsyn till protonens magnetiska moment. Detta kommer ge
$$
E^1 = \frac{\mu_{0}g_{p}e^2}{3\pi m_{p}m_{e}a^3}\langle \mathbf{S}_{p} \cdot \mathbf{S}_{e}  \rangle
$$
då magnetiska momentet är 
$$
\boldsymbol{\mu}_p = \frac{g_p e}{2m_p} \mathbf{S}_p, \quad \boldsymbol{\mu}_e = -\frac{e}{m_e} \mathbf{S}_e
$$
vilket kallas **spinn-spinn koppling**. Det totala spinnet är 
$$
\mathbf{S}=\mathbf{S}_{e}+\mathbf{S}_{p} \implies \mathbf{S}_{p} \cdot \mathbf{S}_{e}=\frac{1}{2}(S^2-S_{e}^2-S_{p}^2)
$$
Energikorrektionen kommer bli
$$
E^1 = \frac{g_p e^2}{3\pi\epsilon_0 m_p m_e c^2 a^3}(\mathbf{S}_p \cdot \mathbf{S}_e) = \frac{4g_p \hbar^4}{3m_p m_e^2 c^2 a^4} \times \begin{cases} +1/4 & \text{(triplett)} \\ -3/4 & \text{(singlett)} \end{cases}
$$
