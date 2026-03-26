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
\Psi(x,t) = \frac{1}{\sqrt{ 2\pi }} \int_{-\infty}^{\infty} \Psi(x)e^{i(kx-\omega t)} \, dk 
$$
## Gaussiska vågpaket
$$
\Psi(x,0)=\left( \frac{2a}{\pi} \right)^{1/4}e^{-ax^2}
$$
Med Fouriertransform:
$$
\implies \Psi(k) = \frac{1}{(2\pi a)^{1/4}}e^{-k^2/4a}
$$
Sats: Lösningar $\Psi$ till SE 
$$
-\frac{\hbar}{2m}\frac{ \partial^2 \Psi }{ \partial x^2 } + V \Psi = E\Psi 
$$
är kontinuerlig i alla punkter $x$ och $\frac{\partial\Psi}{\partial x}$ kontinuerlig utom i punkter där potentialen har ett oändligt steg.
