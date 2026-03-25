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
## Energinivåer
Antag att $\psi$ är en egenfunktion med energiegenvärde $E: H\psi=E\psi$. Då blir 
$$
Ha\psi = (E-\hbar \omega)a\psi \implies a\psi \text{ lösning med energi }E-\hbar \omega.
$$
$$
Ha^{\dagger}\psi = (E+\hbar \omega)a^{\dagger}\psi \implies a^{\dagger}\psi \text{ lösning med energi }E+\hbar \omega.
$$
Vi kan alltså om vi vet en lösning "stega" fram nya lösningar med energiskillnad $\hbar \omega$.
Sats: Energin begränsas underifrån av potentialens minimum. $E \ge V_{min}$.
$\implies$ Det måste finnas ett minsta energiegenvärde $E_{0}$ så att $a\psi_{0}=0$. $H\psi_{0}=E_{0}\psi_{0}$.
$$
H\psi_{0}= \hbar \omega\left( a^{\dagger}a+\frac{1}{2} \right) = \hbar \omega\left( s^{\dagger}\underbrace{ a\psi_{0} }_{ =0 }+\frac{1}{2}\psi_{0} \right)= \frac{\hbar \omega}{2}\psi_{0} = E\psi_{0}
$$
Alltså fås grundtillståndsenergin
$$
E_{0}=\frac{\hbar\omega}{2}.
$$
Genom att $n$ energikvanta $\hbar \omega$ adderas till grundtillståndsenergin fås den $n$:te exciterade energinivån:
$$
E_{n}=\left( n+\frac{1}{2} \right)\hbar \omega, \quad n=0,1,2,3,\dots.
$$
^Energiniva
Vi kommer även få (med normering) att 
$$
\psi_{0}(x)=\left( \frac{m\omega}{\pi \hbar} \right)^{1/4}e^{-m\omega x^2/2\hbar}.
$$
Vi söker de exciterade tillstånden. $\psi_{n} \propto(a^{\dagger})^n\psi_{0}$. $\ket{n}=\ket{\psi_{n}}$. Vi normerar så att
$$
 \text{Sök A: } a\psi_{n}=A\psi_{n-1}
$$
$$
\langle n | a^{\dagger}a | n \rangle=\langle a\psi_{n} | a\psi_{n} \rangle = |A|^2\langle n-1 | n-1 \rangle = |A|^2 \implies a\ket{n} =\sqrt{ n }\ket{n-1}. 
$$
Vidare blir
$$
a^{\dagger}\ket{n} =\sqrt{ n+1 }\ket{n+1}. 
$$
Vi kommer få ett allmäna formeln för exciterade tillstånden
$$
\psi_{n}(x) = \left( \frac{m\omega}{\pi \hbar} \right)^{1/4} \frac{1}{\sqrt{ 2^nn! }}H_{n}(\xi)e^{-\xi^2/2}
$$
där $\xi^2=\frac{m\omega}{\hbar}x^2$ och Hermitepolynomen
$$
H_{0}=1,H_{1}=2\xi,H_{2}=4\xi^2-2,H_{3}=8\xi^3-12\xi\dots
$$
## Klassiskt förbjudna områdena
## Varför viktigt?
$a^{\dagger}, a$ kallas skapelse och förintelseoperatorer inom kvantfältteori.
$$
u=\frac{E}{V}=\frac{1}{2}\varepsilon_{0}\varepsilon^2+\frac{1}{2\mu_{0} }B^2.
$$









