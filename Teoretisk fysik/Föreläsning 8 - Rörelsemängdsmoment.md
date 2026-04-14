$$
\mathbf{L} = \mathbf{r} \times \mathbf{p} = \begin{vmatrix}
\mathbf{e}_{x} & \mathbf{e}_y & \mathbf{e}_{z} \\
x & y & z \\
p_{x} & p_{y} & p_{z}
\end{vmatrix} = (yp_{z}-zp_{y}, zp_{x}-xp_y, xp_{y}-yp_{x}) = (L_{x}, L_{y}, L_{z})
$$
$$
L^2 = L_{x}^2 + L_{y}^2 + L_{z}^2
$$
Banrörelse:
$$
\hat{L}^2 Y^m_{l} = l(l+1)\hbar^2 Y_{l}^m, \quad \hat{L}_{z} Y_{l}^m = m\hbar Y_{l}^m.
$$
Nu:
$$
\hat{L}\ket{lm} = l(l+1) \hbar^2 \ket{lm} , \quad L_{z} \ket{lm} =m\hbar \ket{lm}, \quad l=0, \frac{1}{2}, 1, \frac{3}{2},\dots, \quad m= -l, \dots, l.
$$
## Klassiskt
$$
\dot{\mathbf{L}} = \frac{d}{dt}(\mathbf{r}\times \mathbf{p}) = \underbrace{ \dot{\mathbf{r}}\times \mathbf{p} }_{ =0 }+\mathbf{r}\times \dot{\mathbf{p}} = \mathbf{r}\times \mathbf{F} = \mathbf{N}= \text{ kraftmoment}
$$
Ex: Sfärisk symmetri $V(\mathbf{r}) = V(r)$, potentiella energin beror endast på radiella komponenten. 
$$
\begin{align}
\implies \mathbf{F} = \frac{dV}{dr}\mathbf{e}_{r} = F_{r}\mathbf{e}_{r} \implies \text{centralkraft} \implies \mathbf{N} = \mathbf{r} \times \mathbf{F} = 0 = \dot{\mathbf{L}} \implies \mathbf{L} \text{ bevaras}
\end{align}
$$
## Energin i banrörelsen
För hastighetens radiella och tangentiella komponenter $\mathbf{v}_{r}, \mathbf{v}_{t}$
$$
L = |\mathbf{L}| = |\mathbf{r}\times m\mathbf{v}| = |\underbrace{ \mathbf{r} \times m\mathbf{v}_{r} }_{ =0 } + \mathbf{r} \times m\mathbf{v}_{t}| = mrv_{t} \implies v_{t} = \frac{L}{mr}
$$
$$
\implies T = \frac{1}{2}mv^2 = \frac{1}{2}mv_{r}^2 + \frac{L^2}{2mr^2}
$$
## Kvantmekaniskt
$$
\mathbf{L} = \mathbf{r} \times \mathbf{p} \implies \hat{\mathbf{L}} = \hat{\mathbf{r}}\times \hat{\mathbf{p}} = (\hat{L}_{x}, \hat{L}_{y}, \hat{L}_{y})
$$
$$
\hat{L}^2 = L_{x}^2 + L_{y}^2 + L_{z}^2
$$
Kommutatorerna blir 
$$
[L_x, L_y] = [y p_z - z p_y,\; z p_x - x p_z]
= x p_y \underbrace{[z, p_z]}_{= i\hbar}
+ y p_x \underbrace{[p_z, z]}_{= -i\hbar}
= i\hbar L_z
$$
Liknande fås:
$$
[L_{x},L_{y}] = i\hbar L_{z}, \quad [L_{y}, L_{z}] = i\hbar L_{x}, \quad [L_{z}, L_{x}] = i\hbar L_{y}
$$
$$
\begin{align}
[L^2, L_{z}] &= [L_{x}^2, L_{z}] + [L_{y}^2, L_{z}] + [L_{z}^2, L_{z}] = \{\dots\} =0 \\
\implies [L^2, L_{x}]&=[L^2, L_{y}]=[L^2, L_{y}]=0
\end{align}
$$
Alltså kommuterar $L_{x},L_{y},L_{z}$ inte(inkompatibla) alltså har de olika egenvektorer. $L_{x}, L_{y},L_{z}$ kommuterar dock med $L^2 \implies$ t.ex $L^2, L_{z}$ har **samma** egenvektorer. Vi studerar egenvärdesproblemet för $L^2$ och $L_{z}$. 
$$
L^2\ket{lm} = l(l+1)\ket{lm} , \quad L_{z}\ket{lm} =m\hbar \ket{lm}. 
$$
Lös $l,m$ med stegoperatorer som vi definierar enligt
$$
L_{+} = L_{x} + iL_{y},\quad L_{-} = L_{x} -iL_{y} = L_{+}^{\dagger}
$$
Kommutatorerna blir:
$$
[L_z, L_\pm] = \pm \hbar L_\pm, \quad [L^2, L_\pm] = 0.
$$
$$
L^2 L_{\pm} \ket{lm} = L_{\pm}L^2\ket{lm} =l(l+1)\hbar^2L_{\pm}\ket{lm}. 
$$
Slutsats: $L_{\pm}\ket{lm}$ är nya egenvektorer till $L^2$ med samma egenvärde $l(l+1)\hbar^2$.
$$
L_{z}L_{\pm}\ket{lm} = L_{\pm}\underbrace{ L_{z}\ket{lm} }_{ m\hbar \ket{lm}  }\pm\hbar L_{\pm}\ket{lm} = (m\pm1)\hbar L_{\pm}\ket{lm} 
$$
Slutsats: ger nya egenevektorer med syegade egenvärden $(m\pm 1)\hbar$.
Givet ett värde på $m$ så fås en stege av nya egenvärden, följden måste terminera, annars fårs otiklåtna egenvärden med $m^2 > l(l+1)$.
$$
\begin{align}
\langle ml | L^2 | ml \rangle = l(l+1)\hbar^2 = \langle L_{x}^2  \rangle + \langle L_{y}^2  \rangle +\langle L_{z}^2  \rangle \\
\langle L_{x}^2  \rangle = \langle ml | L_{x}^2 | ml \rangle = \langle L_{x}\psi_{ml} | L_{x}\psi_{ml} \rangle \geq 0.
\end{align}
$$
Alltså finns $m_{max}>m_{min}$ s.a $L_{+}\ket{lm_{max}} =0$, $L_{-}\ket{lm_{min}} = 0$.
Ny identitet:
$$
L_{+}L_{-} = (L_{x}+iL_{y})(L_{x}-iL_{y}) = L_{x}^2 + L_{y}^2 - i\underbrace{ (L_{x}L_{y}-L_{y}L_{x}) }_{ =i\hbar L_{z} } = L^2-L_{z}^2 + \hbar L_{z}
$$
$$
L_{-}L_{+} = L^2 - L_{z} -\hbar L_{z}
$$
$$
\begin{align}
L_{-}L_{+} \ket{lm_{max}} = 0 = (L^2 - L_{z} -\hbar L_{z})\ket{lm_{max}} = (l(l+1)-m_{max}(m_{max}+1))\hbar^2\ket{lm_{max}} \\
  \implies m_{max}=l. 
\end{align}
$$
På samma sätt:
$$
m_{min}=-l
$$
$$
\implies m_{max}-m_{min}=2l = \text{heltal eftersom m tar heltalssteg}
$$
Alltså blir $l$ halvtaligt 
$$
l = 0, \frac{1}{2} , 1, \frac{3}{2},\dots, \quad m=-l, \dots ,l
$$
Vi får alltså nya halvtaliga $l$-värden, $l=\frac{1}{2}, m=\pm \frac{1}{2}$ blir elektronspinn.
Normering:
$$
L_{+}\ket{lm} = A_{+}\ket{l,m+1} \text{ antag normerade ketar}
$$
$$
\begin{align}
\langle lm | L_{+}L_{+} | lm \rangle = \langle L_{-}^{\dagger}\psi_{lm} | L_{+}\psi_{lm} \rangle = |A_{+}|^2= \langle L^2-L_{z}^2 -\hbar L_{z} \rangle = \{ \cdots\}  \\
L_{\pm}\ket{lm} = \sqrt{ l(l+1)-m(m\pm 1) }\hbar \ket{l, (m\pm 1)} 
\end{align}
$$
I $\ket{lm}$ är $L_{z}$ bestämd till $m\hbar$. Men
$$
\Delta L_{x} \Delta L_{y}  \ge \frac{1}{2}[\langle [L_{x}, L_{y}]  \rangle] = \frac{1}{2} m\hbar^2 \implies L_{x},L_{y} \text{ osäkra}.
$$
















