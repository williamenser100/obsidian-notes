[Föreläsningsanteckningar](https://canvas.kth.se/courses/59410/pages/forelasningar-anteckningar-bilder-och-kompletterande-material?module_item_id=1392632)
## Töjningstillstånd (2D/3D)
I varje punkt $(x,y,z)$ tilldelas en förskjutningsvektor $\underset{\sim}{u}=(u,v,w)$ som beskriver hur punkten förflyttas under kroppens deformation.

Vi definierar normaltöjningar för ett visst koordinatsystem enligt (t.ex för $x$,$y$)
$$
\varepsilon_{x} = \frac{ \partial u }{ \partial x } , \quad \varepsilon_{y} = \frac{ \partial u }{ \partial y }
$$
samt skjuvningen enligt 
$$
\gamma_{xy} = \frac{ \partial u }{ \partial y } +\frac{ \partial v }{ \partial x } =\{ \text{ofta är} \} = 2\varepsilon_{xy}. 
$$
$$
\gamma_{yz} = \frac{ \partial u }{ \partial z } +\frac{ \partial w }{ \partial y } = 2\varepsilon_{yz}. 
$$
$$
\gamma_{zx} = \frac{ \partial w }{ \partial x } +\frac{ \partial u }{ \partial z } = 2\varepsilon_{zx}. 
$$
Om vi använder töjningskomponenterna $\varepsilon_{xy}, \varepsilon_{yz}, \varepsilon_{zx}$ så definierar vi den symmetriska töjningsmatrisen (i 3D)
$$
\underset{\sim}{T}=\underset{\sim}{T}^T = 
\begin{bmatrix}
\varepsilon_{x} & \varepsilon_{xy} & \varepsilon_{xz} \\
\varepsilon_{xy} & \varepsilon_{y} & \varepsilon_{yz} \\
\varepsilon_{zx} & \varepsilon_{yz} & \varepsilon_{z}
\end{bmatrix}
$$
där 
$$
\varepsilon_{ij}=\frac{\gamma_{ij}}{2}.
$$
Töjningsmatrisen $\underset{\sim}{T}$ är en tensor, transfomerar som en tensor. Detta betyder att för en snittyta med normal $\underset{\sim}{n}$ så blir 
$$
\varepsilon_{n} = \underset{\sim}{n}^T \underset{\sim}{T}\underset{\sim}{n}, \quad \frac{\gamma_{n}}{2} = \sqrt{ |\underset{\sim}{T}\underset{\sim}{n}|^2-\varepsilon_{n}^2 }.
$$

## Huvudtöjningar
>[!definition]
>**Huvudtöjning**
>En huvudtöjning är en normaltöjning i en riktning längs med vilken ingen skjuvning förekommer. Denna riktning kallas huvudtöjningsriktning.

Det finns alltid $3$ st ortogonala huvudtöjningar $\varepsilon_{1}>\varepsilon_{2}>\varepsilon_{3}$ med huvudtöjningsriktningar $\underset{\sim}{n_{1}}, \underset{\sim}{n_{2}}, \underset{\sim}{n_{3}}$.  Bestäms likt som egenvärdesproblem enligt
$$
[\underset{\sim}{T} - \varepsilon \cdot I]\underset{\sim}{n} = \underset{\sim}{0}.
$$
## Mohrs töjningscirkel

![[Pasted image 20260323093423.png|426]]
Mohrs töjningscirkel plottar alla punkter $(\varepsilon_{x}, \frac{\gamma_{xy}}{2})$ ritas i ett $\varepsilon, \frac{\gamma}{2}$-plan. Då gäller att
- Radien $R$ $\to$ $R=\sqrt{ \left( \frac{\varepsilon_{x}-\varepsilon_{y}}{2} \right)^2 +\left( \frac{\gamma_{xy}}{2} \right)^2}$.
- Mittpunkt $\varepsilon _m=\frac{\varepsilon_{x}-\varepsilon_{y}}{2}$.
- Tillståndet då vi i koordinatsystemet roterat moturs $\varphi$ från x-axeln fås genom att rotera diametern i Mohrs cirkel med $2\varphi$ åt motsatt håll (medurs).
- Huudtöjningarna kan bestämmas enligt $\varepsilon_{1,2}=\varepsilon_{m} \pm R$.

## Hookes generaliserade lag
Fås genom att superponera enaxligt i flera riktningar
$$
\begin{aligned}
\varepsilon_{x}&=\frac{1}{E}[\sigma_{x}-\nu \sigma_{y}-\nu \sigma_{z}] +\alpha \Delta T \\
\varepsilon_{y}&=\frac{1}{E}[-\nu\sigma_{x}+ \sigma_{y}-\nu \sigma_{z}] +\alpha \Delta T \\
\varepsilon_{x}&=\frac{1}{E}[-\nu\sigma_{x}-\nu \sigma_{y}+ \sigma_{z}] +\alpha \Delta T
\end{aligned}
$$
samt
$$
\gamma_{xy}=\frac{\tau_{xy}}{G}, \quad \gamma_{xz}=\frac{\tau_{xz}}{G}, \quad \gamma_{yz}=\frac{\tau_{yz}}{G}.
$$





