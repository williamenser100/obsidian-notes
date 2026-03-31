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
Hela lösningen är då är då klotfunktioner
$$
Y_{m}^l = P_{l}^m (\cos \theta) e^{im\phi}.
$$
Normerade så att
$$
\int_{0}^{2\pi} \int_{0}^\pi [Y_{l'}^{m'}]Y_{l}^m \sin\theta d\theta d\phi = \delta_{ll'}\delta_{mm'}.
$$
Allmänng lösning
$$
Y(\theta, \phi) = \sum_{lm} c_{lm} Y_{l}^m
.$$
## Radiella ekvationen
$$
\frac{1}{R}\frac{d}{dr}\left(r^2\frac{dR}{dr}\right)
- \frac{2mr^2}{\hbar^2}[V(r)-E]
= l(l+1)R
$$
Vi måste välja en potential för att lösa för $R$, vi väljer Couloumb potentialen
$$
V(r) = -\frac{e^2}{4\pi\epsilon_{0}r}.
$$
Förenkla med variabelsubstitution $u(r)=R(r)r$, ger
$$
-\frac{\hbar^2}{2m} \frac{d^2u}{dr^2} + \underbrace{ \left[ V(r) + \frac{\hbar^2}{2m} \frac{l(l+1)}{r^2} \right] }_{ =V_{eff} }u = Eu
$$

Vi söker bundna tillstånd $E<V(r=\infty) =0$ alltså atomära tillstånd där partikeln bunden till kärnan.
Inför
$$
E=\frac{\hbar^2k^2}{2m},\quad \rho=kr, \quad \rho_0=\frac{me^2}{2\pi\epsilon_{0}\hbar^2k}.
$$
$$
\begin{align}
\implies \frac{d^2u}{d\rho^2} + \left( 1-\frac{\rho_{0}}{\rho} + \frac{l(l+1)}{\rho^2} \right)u = 0.
\end{align}
$$
I gränsen $\rho \to \infty$ blir
$$
\frac{d^2u}{d\rho^2} = u \implies u=Ae^{-\rho} + B\underbrace{ e^\rho }_{ \to \infty \implies B=0 }.
$$
Då $\rho \to 0$ blir
$$
\frac{d^2u}{d\rho^2} = \frac{l(l+1)}{\rho^2}u \implies u = C\rho^{l+1} + D\underbrace{  \rho^{-l}  }_{ \to \infty \implies D=0  }.
$$
$$
\begin{align}
\implies u &= v(\rho) e^{-\rho} \\
\implies v''& -2v' + \frac{\rho_{0}}{\rho}v + \frac{l(l+1)}{\rho^2}v=0 \implies \text{potenserieansats} \\
v&=\sum_{j=0}^\infty c_{j} \rho^{j+l+1} \implies c_{j+1} = \frac{2(j+l+1)-\rho_{0}}{(j+1)(j+2l+2)}c_{j}
\end{align}
$$
Potensserie måste terminera till ändliga polynom $\implies \exists$ största värde $j=j_{\text{max}}$ så att $c_{j_{max}+1}=0$. Definiera $n=j_{max} + l + 1$ som vi kallar för **huvudkvanttalet**. Kvanttalen är då
$$
\begin{align}
n&=1,2,3\dots \\
l&=0,1,\dots,n-1 \\
m&=0,\pm1, \pm 2, \dots
\end{align}
$$
Samt får vi
$$
\rho_{0} = 2n = \frac{me^2}{2\pi\epsilon_{0}\hbar^2k} \implies k_{n} = \frac{me^2}{2\pi\epsilon_{0}\hbar^2 n} = \frac{1}{2n}
$$
där vi infört Bohrradien $a$
$$
a = \frac{4\pi\epsilon_{0}\hbar^2}{me^2} = 0.529 \text{ Å}.
$$
$$
E_{n} = \frac{E_{1}}{n^2}, n=1,2,3,\dots, \quad E_{1} = -\frac{m}{2\hbar^2} \left( \frac{e^2}{4\pi\epsilon_{0}} \right)^2 = -13.6 \text{ eV}.
$$







