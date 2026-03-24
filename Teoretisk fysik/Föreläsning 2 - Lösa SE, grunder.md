## Kvantmekanik
Vågfunktion för fria partiklar i planvåg $\Psi(x,t)=Ae^{i(kx-\omega t)}$. Intensiteten
$$
\begin{aligned}
I\propto |\Psi|^2 = |\Psi_{1}+\Psi_{2}|^2 = |Ae^{i(kr_{1}-\omega t)} + Ae^{i(kr_{2}-\omega t)}|^2 = |A|^2|e^{-i\omega t}|^2 |e^{ikr_{1}e^{ikr_{2}}}|^2 = \\=|A|^2(e^{ikr_{1}}+e^{ikr_{2}}) (e^{-ikr_{1}}+e^{-ikr_{2}}) \propto 1+1+e^{ik(r_{1}-r_{2})} + e^{-ik(r_{1}-r_{2})} = 2 + \cos{k(r_{1}-r_{2})}
\end{aligned}
$$
som har max (då $k=\frac{2\pi}{\lambda}$) för $r_{1}-r_{2}=n\lambda$. 

Grundantaganden:
Planck-Einstein, varje partikel har en energi enligt $E=\hbar \omega$. $\left( \hbar =\frac{h}{2\pi} \right)$.
De Broglie, varje partikel har en rörelsemängd enligt $p=\hbar k=\frac{2\pi \hbar}{\lambda}=\frac{h}{\lambda}$.

Observabler: kvantiteter som mätts i experiment. Representeras av operatorer i kvantmekaniken. Operator tar en vågfunktion $\to$ ny vågfunktion.
Operatorer
- Position $x$, positionsoperator $\hat{x}=x$ $\to$ $\hat{x}\Psi =\hat{x}\Psi$ 
- Rörelsemängd $p$, $\hat{p}=\frac{\hbar}{i} \frac{\partial}{\partial x}$.
- $H=\frac{p^2}{2m}+V(x) \Longrightarrow$   $\hat{H} = -\frac{\hbar^2}{2m} \frac{\partial^2}{\partial x^2} + V(x)$.
För plan våg fås ett egenvärdesproblem för operatorn $\hat{p}$
$$
\hat{p} \Psi = \frac{\hbar}{i} \frac{\partial}{\partial x}Ae^{i(kx-\omega t)} = \frac{\hbar}{i} ik \Psi = \hbar k \Psi = p\Psi.
$$
Nu för hamiltonoperatorn
$$
H=E \to \hat{H} = \frac{\hat{p}^2}{2m} \Psi + V(\hat{x})\Psi = i\hbar \frac{\partial\Psi}{\partial t}
$$
vilket är Schrödingerekvationen.
#### Tolka vågekvationen
Vet inte vad vågekvationen $\Psi$ betyder fysikaliskt. 
$|\Psi|^2$ ger sannolikhetstätheten, $|\Psi|^2 \Delta x$ av en positionsmätning ger sannolikheten att hitta partikeln inom området $\Delta x$.  

#### Väntevärden
Medelvärden kallas väntevärden:
$$
\langle x \rangle = \int_{-\infty}^{\infty} \Psi ^* \hat{p} \Psi dx, \quad \langle H \rangle = \int_{-\infty}^{\infty} \Psi ^* \hat{H} \Psi dx
$$
^Vantevarde

Standardavvikelsen kallas osäkerheten:
$$
\Delta x = \sqrt{ \langle x^2 \rangle - \langle x \rangle ^2 }, \quad \Delta p = \sqrt{ \langle p^2 \rangle - \langle p \rangle ^2} = \int_{-\infty}^{\infty} \Psi ^* \hat{p}^2 \Psi dx.
$$
^Standardavvikelse


Osäkerhetsprincip $\Delta x \Delta p  \ge \frac{\hbar}{2}$, utesluter klassiska exakta banor.
#### Ehrenfests teorem
Väntevärdena rör sig klassiskt: 
$$
\langle p \rangle = m \frac{d\langle x \rangle }{dt}
$$
^Ehrenfest
som motsvarar det klassiska $p=mv$.
$$
\frac{d\langle p \rangle}{dt} = \left\langle  - \frac{\partial V}{\partial x} \right\rangle 
$$
motsvarar klassiska $\dot{p} = F$.
Slutsats: med operatorandet återfås klassisk mekanik. 
Makroskopiska system: $\Delta x, \Delta p$ oobserverbart små.

#### Vägintegraler
Sannolikheten att gå från $x(t_{1})$ till $x(t_{2})$ ges av absolutbeloppet i kvadrat av
$$
\sum_{\text{alla vägar}} e^{\frac{i}{\hbar}S}.
$$
#### Tidsoberoende SE
Antag $V(x,t)$ oberoend av $t$: $V(x)$. $\to$ SE separabel. 
Produktansats $\Psi(x,t)=\psi(x)e^{-i\omega t}$. Insatt ger tidsoberoende SE
$$
- \frac{\hbar^2}{2m} \frac{\partial^2\psi(x)}{\partial x^2} + V(x) \psi(x) = E\psi(x).
$$
^Tidsoberoende-SE
$\hat{H} \psi = E\psi$ lösningar egenfunktioner $\psi_{n}(x)$ egenvärden $E_{n}$. Då blir 
$$
\Psi_{n}(x,t) = \psi_{n}(x) e^{-i\omega_{n}t}, \quad E_{n} = \hbar \omega _{n}.
$$
$\Psi$ har tidsoberoende sannolikhetstäthet!
$$
|\Psi(x,t)|^2 = |\psi_{n}|^2 |e^{-iEt/\hbar}|^2 = |\psi_{n}|^2.
$$
$\psi_{n}$: stationära tillstånd. Så var kommer tidsberoende ifrån?
Tidsberoende kommer från superpositioner, t.ex 
$$
\Psi(x,t)=\frac{\psi_{1}(x)e^{-i\omega_{1}t} + \psi_{2}(x)e^{-i\omega_{1}t}}{\sqrt{ 2 }}
$$
kommer ge att sannolikheten $|\Psi(x,t)|^2$ kommer att oscillera med en term $\cos{(\omega_{2}-\omega_{1}})t$ med tiden.

#### Oändlig lådpotential
Vi definierar potentialen som kan modellerar t.ex elektroner i metaller
$$
V(x) = \begin{cases}
  0  & 0<x<L \\
  \infty  & \text{för övrigt}
\end{cases}
$$
Vi ska då lösa $\hat{H} \psi_{n} = E_{n}\psi_{n}$, det visar sig att vi får lösning $\Psi(x,t)=\psi(x)e^{-iE_{nt/\hbar}}$
$$
\psi_{n} = \sqrt{ \frac{2}{L} } \sin{k_{n}x}, \quad k_{n} = \frac{n\pi}{L}, n = 0,1,\dots, \quad E_{n}=\frac{\hbar^2k_{n}^2}{2m}.
$$
^Losning-oandlig-ladpotential
Där $\psi_{n}, \psi_{m}$ är ortogonala för alla $n,m$.
