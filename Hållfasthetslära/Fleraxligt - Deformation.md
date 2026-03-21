[Föreläsningsanteckningar](https://canvas.kth.se/courses/59410/pages/forelasningar-anteckningar-bilder-och-kompletterande-material?module_item_id=1392632)
### Töjningstillstånd (2D/3D)
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
Töjningsmatrisen $\underset{\sim}{T}$ är en tensor, transfomerar som en tensor.

