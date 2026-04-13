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
[L^2, L_{z}] = [L_{x}^2, L_{z}] + [L_{y}^2, L_{z}] + [L_{z}^2, L_{z}] =  \\

\end{align}
$$







