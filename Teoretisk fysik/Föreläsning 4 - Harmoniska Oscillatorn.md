## Klassiskt

## Kvantmekaniskt
Ska lösa tisoberoende SE
$$
\frac{\hat{p}^2}{2m}\psi+\frac{1}{2}m\omega^2x^2 \psi = E\psi(x)
$$
Som löses med Diracs algebraiska lösningsmetod, idén:
$$
p^2+x^2 = (-i p + x)(i p + x) \approx a^{\dagger}a
$$
som ska likna faktorn $p^{\dagger}p$ i energin för fria partikeln. Definiera stegoperatorer
$$
\begin{dcases}
a = \frac{1}{\sqrt{ 2\hbar m\omega }}(i p + m \omega x)\\
a^{\dagger} = \frac{1}{\sqrt{ 2\hbar m\omega }}(-i p + m \omega x)\\
\end{dcases} \implies
\begin{dcases}
x=\sqrt{ \frac{\hbar}{2m\omega} }(a^{\dagger}+a) \\
p = i \sqrt{ \frac{m\omega \hbar}{2} }(a^{\dagger}-a)
\end{dcases}
$$
^Stegoperator
$a$ kallas sänkningsoperatorn $a^{\dagger}$ höjningsoperatorn.

## Kommutatorer
Definiera kommutatorn mellan två operatorer $A,B$ som 
$$
[A,B] = AB-BA.
$$
^Kommutatorn
Egenskaper:
$$
[A,A]=0, \quad [A,I]=0, \quad [A,B] = -[B,A]
$$
$$
[AB,C] = A[B,C]+[A,C]B, \quad [A,BC] = B[A,C]+[A,B]C.
$$
Position och rörelsemängd:
$$
[x,p]\psi=xp\psi-px\psi=xp\psi-xp\psi+i\hbar\psi \implies[x,p]=i\hbar.
$$
Vi kan även skriva
$$
H = \left( a^{\dagger}a+\frac{1}{2} \right)\hbar \omega=\left( N+\frac{1}{2} \right)\hbar \omega.
$$
$$
[a,a^{\dagger}]=I.
$$
$$
[H,a^{\dagger}]=h\omega a^{\dagger}, \quad [H,a]=-\hbar \omega a.
$$

