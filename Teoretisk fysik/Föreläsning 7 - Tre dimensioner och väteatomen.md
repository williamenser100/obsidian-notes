## Tre dimensioner
$$
x \to \mathbf{r} = (x,y,z)
$$
$$
p = \frac{\hbar}{i} \frac{ \partial  }{ \partial x } \to \mathbf{p}=(p_{x}, p_{y}, p_{z}) = \frac{\hbar}{i}\left( \frac{ \partial  }{ \partial x }, \frac{ \partial  }{ \partial y } \frac{ \partial  }{ \partial z }   \right) = \frac{\hbar}{i} \nabla
$$
$$
H = -\frac{\hbar}{2m}\frac{ \partial^2 }{ \partial x^2 } +V(x) \to H = -\frac{\hbar^2}{2m} \nabla^2 + V(\mathbf{r}).
$$
## Exempel
Antag att egenfunktionerna till SE är $\psi_{x,m}(x), \psi_{y,n}(y)$, egenfunktioner och egenvärden är då
$$
\psi(mn)(x,y) = \psi_{x,m}(x)\psi_{y,n}(y), \quad E_{mn} = E_{x,m} + E_{y,n}
$$
Allmänna lösningen har formen
$$
\Psi(x,y,t) = \sum_{m,n} c_{mn}\psi_{x,m}(x) \psi_{y,n}(y)e^{-iE_{mn}t/\hbar}.
$$
Eller på vektorform skrivs basvektorerna som en tensorprodukt
$$
\ket{\psi_{mn}} = \ket{mn} = \ket{m} \otimes \ket{n}.   
$$
## SE i sfäriska koordinater
$$
\begin{align}
 -\frac{\hbar}{2m}\nabla^2 & \psi+ V \psi = -\frac{\hbar^2}{2m} \left[ \frac{1}{r^2} \frac{ \partial  }{ \partial r } \left( r^2\frac{ \partial \psi }{ \partial r }  \right) + \frac{1}{r^2\sin \theta} \frac{ \partial  }{ \partial \theta } \left(\sin \theta \frac{ \partial \psi }{ \partial \theta }\right) \frac{1}{r^2\sin^2\theta} \frac{ \partial^2 \psi }{ \partial \phi^2 }  \right]  \\
+V(r) \psi &= E\psi(\mathbf{r}).
\end{align}
$$
Separera variabler
$$
\psi = R(r)Y(\theta,\phi).
$$
Insatt kommer ge 
$$
\begin{align}
\frac{1}{R}\frac{d}{dr}\left(r^2\frac{dR}{dr}\right)
- \frac{2mr^2}{\hbar^2}[V(r)-E]
&= -\frac{1}{Y}
\left[
\frac{1}{\sin\theta}\frac{\partial}{\partial\theta}
\left(\sin\theta \frac{\partial Y}{\partial\theta}\right)
+
\frac{1}{\sin^2\theta}\frac{\partial^2 Y}{\partial\phi^2}
\right]  \\
&= \text{konstant} = l(l+1)
\end{align}
$$

## Banrörelse
Den vinkelberoende delen av rörelsen kallas banrörelsen:
$$
\sin\theta \frac{ \partial  }{ \partial \theta } \left( \sin \theta \frac{ \partial Y }{ \partial \theta }  \right) + \frac{ \partial^2 Y }{ \partial \phi^2 } + l(l+1)\sin^2\theta \ Y =0
$$
Separation enligt $Y = \Theta(\theta)\Phi(\phi)$ kommer ge $\Phi$ lösningen som
$$
\Phi(\phi) = e^{im\phi}
$$
Kontinuerlig i $\phi=2\pi$ ger $m=0,\pm 1, \pm 2,\dots$
Lösningen till $\theta$-ekvationen kommer med potensserieansats ge lösningar som polynom
$$
\Theta(\theta) = AP_{l}^m(x)
$$






