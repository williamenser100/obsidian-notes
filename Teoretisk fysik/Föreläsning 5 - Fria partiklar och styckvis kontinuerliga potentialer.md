## Styckvis konstanta potentialer
Idé : byt varierande potential mot styckvis kontinuerlig potential. Denna modell är bra om $\delta x$=$x$-intervallet där potentialen varierar är 
$$
\delta x \ll \lambda = \frac{h}{p}.
$$
alltså bra om $p$ är liten, typiskt om för låga energier, $E$ är liten.
## Fria partiklar
$$
V(X)= 0,  \forall x.
$$
Plana vågor $\Psi(x,t)=Ae^{i(kx-\omega t)}$ är egenfunktioner till $\hat{p}$ och $\hat{H}$. Alltså
$$
\hat{p} \Psi=\frac{\hbar}{i}\frac{ \partial  }{ \partial x } \Psi=\hbar k\Psi=p\Psi
$$
$$
\hat{H}\Psi=\frac{\hat{p}^2}{2m}\Psi = \frac{\hbar^2k^2}{2m}\Psi=\frac{p^2}{2m}\Psi=E\Psi.
$$
Dispersionsrelationen $\omega(k)=\frac{\hbar k^2}{2m}$.
Sannolikhetsström def:
$$
j=\frac{\hbar}{2mi}\left( \Psi^*\frac{ \partial \Psi }{ \partial x } -\Psi \frac{ \partial \Psi^* }{ \partial x }  \right) = \frac{\hbar k}{m}|\Psi|^2 =\frac{p}{m}|\Psi|^2.
$$
Motsvarar klassisk strömtäthet.
## Vågpaket
Plan våg modellerar partikelstråle = ström i $-\infty<x<\infty$.
Plana vågor är icke normerbara ty
$$
\int_{-\infty}^{\infty} |\Psi|^2 \, dx =|A|^2\int_{-\infty}^{\infty} 1 \, dx = ??
$$
Fysikaliska tillstånd är normerbara i vågpaket
$$
\Psi(x,t=0)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty} \Psi(k)e^{ikx} \, dk,\quad \Psi(k) = \frac{1}{\sqrt{ 2\pi }} \int_{-\infty}^{\infty} \Psi(x,0)e^{-ikx} \, dx 
$$
(Finns ingen kvantisering för fria partiklar, endast för bundna partiklar)
Tidsutvecklingen för vågpaketet blir då 
$$
\Psi(x,t) = \frac{1}{\sqrt{ 2\pi }} \int_{-\infty}^{\infty} \Psi(k)e^{i(kx-\omega t)} \, dk 
$$
## Gaussiska vågpaket
$$
\Psi(x,0)=\left( \frac{2a}{\pi} \right)^{1/4}e^{-ax^2}
$$
 Med Fouriertransform:
$$
\implies \Psi(k) = \frac{1}{(2\pi a)^{1/4}}e^{-k^2/4a}
$$
#### Kontinuitetsvillkor på vågfunktionen
Sats: Lösningar $\Psi$ till SE 
$$
-\frac{\hbar}{2m}\frac{ \partial^2 \Psi }{ \partial x^2 } + V \Psi = E\Psi 
$$
är kontinuerlig i alla punkter $x$ och $\frac{\partial\Psi}{\partial x}$ kontinuerlig utom i punkter där potentialen har ett oändligt steg.
Ex:
Delta funktionspotential $V(x)=-\alpha \delta(x)$ med Dirac delta funktion.

För $x=0$ : $-\frac{\hbar}{2m}\frac{ \partial^2 \Psi }{ \partial x^2 } = E\Psi$. Sök bundna tillstånd: $E <V(x) : x=\pm \infty$ där $E<0$.
Fall 1 : Spridningstillstånd : $E>0$
$$
\Psi'' = \frac{2m(-E)}{\hbar^2}\Psi = \kappa^2 \Psi, \quad \kappa^2 = \frac{2m(-E)}{\hbar^2}, \quad E=-\frac{\hbar \kappa^2}{2m}.
$$
$$
\implies \Psi(x)=Ae^{-\kappa x}+Be^{\kappa x} \to 0 \text{ för } x \to \pm \infty 
$$
$$
\Psi=\begin{dcases}
Ae^{-\kappa x}, &x>0 \\
Be^{\kappa x}, & x<0
\end{dcases}
$$
RV $\implies A=B = \Psi(0)$ 
$$
\implies \Psi(x) = Ae^{-\kappa |x|}.
$$
Slutsats : oberoende av styrkan $\alpha$ finns exakt ett bundet tillstånd.
## Tunnling, rektangulär potentialbarriär
Där $0<E<V_{0}$:
$$
V(X) = \begin{dcases}
V_{0} > 0, & |x|<a \\
0, & |x|>a
\end{dcases}
$$
$x<-a$:
$$
-\frac{\hbar}{2m}\frac{ \partial^2 \Psi }{ \partial x^2 } = E\Psi \implies \Psi'' = -\frac{2mE}{\hbar^2}\Psi = -k^2\Psi \implies \Psi=Ae^{ikx} + Be^{-ikx}.
$$
$|x|<a$:
$$
		-\frac{\hbar}{2m}\frac{ \partial^2 \Psi }{ \partial x^2 } + V_{0} \Psi = E\Psi \implies \Psi'' = \frac{2m(V_{0}-E)}{\hbar^2}\Psi = \kappa^2\Psi
$$
$$
\implies \Psi=Ce^{\kappa x}+De^{-\kappa x}
$$
$x>a$:
$$
\implies \Psi = Fe^{ikx} + 0 e^{-ikx} = Fe^{ikx} \text{ ty ingen inkommande stråle}.
$$
Kontinuitet i $x=\pm a$ alltså att $\Psi$ och $\Psi'$ är kontinuerliga i $\pm a$ ger fem obekanta men endast fyra ekvationer.
Vill veta transmissions och reflektionssannolikhet.
$$
T = \left|\frac{F}{A}\right|^2
= \frac{1}{1 + \frac{V_0^2}{4E(V_0 - E)}
\sinh^2\!\left(
\frac{2a}{\hbar}\sqrt{2m(V_0 - E)}
\right)}
$$
Alltså kan partiklar transmitteras med sannolikhet som inte är noll för $E<V_{0}$!

Om $E>V_{0}$ så blir liknande:
$$
T = \frac{1}{1+\frac{V_{0}^2}{4E(E-V_{0})}\sin^2\tilde{\kappa}L}.
$$
Vilket ger 
$$
T \sim e^{-2\kappa L}.
$$


