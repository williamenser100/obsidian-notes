[Föreläsningsanteckningar](https://canvas.kth.se/courses/59410/pages/forelasningar-anteckningar-bilder-och-kompletterande-material?module_item_id=1392632)
Utmattning är brott som uppstår vid cyklisk belastning. Antal cykler till brott $N$ används för att kvantifiera livslängden.
Wöhlerkurva plottar total livslängd $N$ mot lastnivån $\sigma$.
![[Pasted image 20260418130904.png|412]]
LCF - low cycle fatigue. HCF - high cycle fatigue.
## Lastbeskrivning
![[Pasted image 20260418130649.png|588]]
Mittspänningen
$$
\sigma_{m} = \frac{\sigma_{max}+\sigma_{min}}{2}
$$
Spänningsamplitud:
$$
\sigma_{a} = \frac{\sigma_{max}-\sigma_{min}}{2}
$$
Spänningsförhållande:
$$
R = \frac{\sigma_{min}}{\sigma_{max}}
$$
Oändligt liv ges för växlande samt pulserande fall. För växlande
$$
\sigma(t) = \pm \sigma_{a}, \quad \sigma_{m}=0, \quad R=1
$$
För pulserande
$$
\sigma(t) = \sigma_{a}\pm\sigma_{a}, \quad \sigma_{m} = a, \quad R=0
$$
## Experimentella utmattningsgränser
För växlande respektive pulserande
$$
\sigma_{u} \text{ växlande}, \quad \sigma_{up} \text{ pulserande}.
$$
Andra lastfall $(\sigma_{a}, \sigma_{m})$ fås med Haigh diagram
![[Pasted image 20260418132105.png|509]]
Haigh diagram gäller för laboratorie miljö/ under perfekta för förhållanden. För verkligheten gäller ofta mycket sämre förhållanden. Haigh diagrammet reduceras med en reduktionsfaktor
$$
\frac{\lambda}{K_{d}K_{r}K_{f}} \le 1
$$
där $\lambda$ - teknologiskt volymsberoende, $K_{d}$ - geometriskt volymsberoende, $K_{r}$ - ytbeskaffenhet, $K_{f}$ - anvisningsverkan s.k reduktionsfaktorer. 
![[Pasted image 20260418132628.png|519]]
## Reduktionsfaktorer
### $\lambda$ - Teknologiskt volymsberoende
Gäller endast gjutna produkter, annars $\lambda=1$. Beror av brottsgränsen $\sigma_{b}=R_{m}$.
### $1/K_{d}$ - Geometriskt volymsberoende
Vid spänningsgradienter vid t.ex böjning och vridning. Beror på 
- Material dimension
- Materialets brottgräns $\sigma_{b}=R$.
### $1/K_{r}$ - Ytbeskaffenhet
Beskrivs mha medelytavvikelse $R_{a}$. Ojämn yta $\implies$ högra $R_{a}$ värde betyder fler defekter/ ojämnheter vilket reducerar utmattninsgränsen. beror av 
- $R_{a}$ värdet
- Materialets brottgräns
### $1/K_{f}$ - Anvisningsverkan
Spänningskoncentration pga geometriändring, hål spår, m.m. Där har man med spänningskoncentrationsfaktorn $K_{t}$
$$
\sigma_{max} = K_{t}\ \sigma_{\text{nom}}. 
$$
Lokal spänningsgradient dvs i liten volym blir högt belastad. Man beräknar då anvisningsfaktorn $K_{f}$ som är motsvarande spänningskoncentrationsfaktor för utmattning enligt
$$
K_{f} = 1 + q(K_{t}-1)
$$
där $q$ - kälkänslighetsfaktor $\le 1$. $q$ beror av 
- Kälradie $\rho$ 
- Materialets brottsgräns $\sigma_{b}$.
Spänningskoncentrationsfaktorn uppstår pga lokal geometri vid inåtgående hörn/ radie.  Skarpare hörn/ mindre radie $\implies$ högra $K_{t}$ och därmed högre $\sigma_{\text{max}}$. 

## Beräkningsgång
1. Ta fram materialdata för rådande belastningstyp:
	- Drag - $\sigma_{u}$, $\sigma_{up}$
	- Böj - $\sigma_{ub}$, $\sigma_{ubp}$
	- Vrid - $\tau_{uv}$, $\tau_{uvp}$
	Samt $\sigma_{b}=R$, $\sigma_{s}$, $\tau_{b}=\sigma_{b}/2$.
2. 


