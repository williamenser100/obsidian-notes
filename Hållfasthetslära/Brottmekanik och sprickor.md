Brottmekanik/ beteende beror av material, men även temperatur, lasthastighet, geometri, spänningstillstånd, kemisk miljön, osv.
Två typer, segt och sprött:
**Sprött** (klyvbrott): Inträffar utan märkbar plastisk deformation, typiskt keramik, glas.

**Segt** (duktilt): föregås av omfattande plastisk deformation innan brottet. Ofta midjebildning. 

### Inverkan av anvisningar/sprickor
Bara för att det är samma area betyder inte att brottbeteendet blir samma. De tre fallen (med samma skuggade tvärsnittsarea) nedan kommer bete sig olika.
![[Pasted image 20260421144345.png]]
Bättre $\implies$ Värre
## Strukturer med anvisningar
Exempel:
![[Pasted image 20260421145555.png]]
I sista fallet blir
$$
\sigma_{max} = \lim_{ \rho \to 0 } \sigma_{\infty}\left( 1+2\sqrt{ \frac{a}{\rho} } \right) \to \infty.
$$
Ger inte så mycket info va...
## Brottkriterier:
Vid icke skarpa anvisningar, så beskrivs spänningen lokalt av $K_{t}$. Vid skarpa sprickor har vi oändlig spänning?
Slutsats: Vid skarpa sprickor kan vi inte bestämma ett brottkriteria i form av spänningar.
Analyseras med brottmekanik - metod/teori för att avgöra när en existerande spricka börjar "växa"(egentligen rusa). 
Belastningen lokalt på sprickan beskrivs av spänningsintensitetsfaktorn, $K_{I}$. 
## Spänningstillståndet nära en sprickspets
Spänningsintensitetsfaktiorn $K_{I}$ är ett skalärt mått på hur materialet vid sprickspetsen belastas. $K_{I}$ har fysikalisk dimension (kraft/area)$\sqrt{ \text{längd} }$. Anges i $MPa\sqrt{ m }$. 
Rakt framför sprickan så blir på x-axeln med $r=x$:
$$
\sigma_{y}(x) = \frac{K_{I}}{\sqrt{ 2\pi x }}
$$
Magnituden/ intensiteten sätts av värdet på $K_{I}$.
Spänningsintensitetsfaktorn $K_{I}$ beror linjärt av yttre lasten, men även av geometrin enligt en principiell formel.
$$
K_{I} = \sigma_{o}\sqrt{ \pi a } \cdot f(\text{geometrin, lastfall})
$$
$a$ är spricklängden, $\sigma_{0}$ är nominell spänning och $f$ är en dimensionslös funktion. 

Yttre lasts påverkan på tillståndet vid sprickan bestäms entydigt av värdet på $K_{I}$. 
$\implies$ Brottvillkor 
$$
K_{I} = K_{Ic}
$$
där $K_{Ic}$ är en materialparameter (tab 33.6). 
### Brottvillkor - giltighet
Linjärelastisk brottmekanik (LEFM) begränsas av plastisk deformation. Experiment visar att om
$$
\min{(a,W-a)} \ge 2.5 \left( \frac{K_{Ic}}{\sigma_{s}} \right)^2
$$
där $a$ är spricklängden och $W$ är bredden så kan LEFM tillämpas. Kallas ASTM-villkoret.

![[Pasted image 20260427093018.png]]

### Spricktillväxt vid cykliskt fall
Gradvis tillväxt vid belastning där $K_{I} < K_{Ic}$ - utmattningsfenomen. 
Fall 1 FS s 266:
$$
K_{I} = \sigma(t) \sqrt{ \pi a } f_{1}\left( \frac{a}{W} \right)
$$
där
$$
\sigma(t) = \sigma_{m} + \sigma_{q}\sin \omega t
$$
$f_{1}$ ökar med $a$ $\implies$ $K_{I}$ ökar med $a$. Om $a$ ökar (dvs sprickan växer) då ökar också $K_{I,max}$ per cykel($N$).
Spricktillväxten, $a(N)$, beskrivs väl av Paris lag:
$$
\frac{da}{dN} = C(\Delta K_{I})^n
$$
där $C,n$ är experimentellt bestämda materialparametrar. 
$$
\Delta K_{I} = 
\begin{dcases}
K_{I,max} -K_{I,min} & K_{I,min}>0\\
K_{I,max} & K_{I,min}<0\\
0, & K_{I,max} < 0
\end{dcases}
$$


