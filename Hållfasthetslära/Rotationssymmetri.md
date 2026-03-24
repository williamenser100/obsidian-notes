[Föreläsningsanteckningar](https://canvas.kth.se/courses/59410/pages/forelasningar-anteckningar-bilder-och-kompletterande-material?module_item_id=1392632)
## Tunnväggiga tryckkärl
Tunn $(h \ll \varnothing D)$, spänningar konstanta i godset.
Betrakta tunnväggigt slutet cylindriskt tryckkärl med radie $a$, godtjocklek $h$ samt inre övertryck $p$ kraft/area. Då gäller att
$$
\begin{align}
\sigma_{\varphi} &= \frac{pa}{h} \\
\sigma_{z} &= \frac{pa}{2h} \\
\sigma_{r} &= 0  
\end{align}
$$
Liknande blir för sfäriskt tryckkärl
$$
\sigma_{\varphi} = \sigma_{\theta} = \frac{pa}{2h}, \quad \sigma_{r} = 0.
$$
Ovan beskriver huvudspänningstillstånd $\tau_{\varphi z}=0,\tau_{\varphi\theta}=0$.
## Rotationssymmetriska tillstånd
Jämvikt:
$$
\frac{ \partial \sigma_{r} }{ \partial r } +\frac{\sigma_{r}-\sigma_{\varphi}}{r}=0 \implies \frac{ \partial (r\sigma_{r}) }{ \partial r }-\sigma_{\varphi} 
$$
Kompatibilitet: Förskjutningar $u_{r}(r)$ enbart i $r$-led.
$$
\varepsilon_{r}=\frac{ \partial u_{r} }{ \partial r } , \quad \varepsilon_{\varphi}=\frac{u_{r}}{r}.
$$
Konstitutivt samband:
$$
\varepsilon_{r}=\frac{1}{E}[\sigma_{r}-\nu\sigma_{\varphi}], \quad \varepsilon_{\varphi} = \frac{1}{E}[\sigma_{\varphi}-\nu \sigma_{r}].
$$
### Allmän lösning
Vi får att allmänna lösningen (2D) för rotationssymmetriska tillstånd:
$$
\sigma_{r}=A-\frac{B}{r^2}, \quad \sigma_{\varphi}=A+\frac{B}{r^2}, \quad u_{r} = \frac{r}{E}[\sigma_{\varphi}-\nu(\sigma_{r}-\sigma_{z})]
$$
där konstanter $A$ och $B$ bestäms av randvillkor $\sigma_{r}$ eller $u_{r}$. Ovan lösning kan användas för att lösa:
- Tunna skivor
- Långa rör
- Tjockväggiga tryckkärl
- $\sigma_{z}$ bestäms av jämvikt i $z$-led.