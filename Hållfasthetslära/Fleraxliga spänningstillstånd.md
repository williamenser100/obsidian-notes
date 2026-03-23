[Föreläsningsanteckningar](https://canvas.kth.se/courses/59410/files/10015052?wrap=1)
För fleraxliga spänningstillstånd samlas alla komponenter i spänningsmatrisen $\underset{\sim}{S}$ som i 3D definieras som:
$$
\underset{\sim}{S} = \begin{bmatrix}
\sigma_{x} & \tau_{xy} & \tau_{xz}  \\
\tau_{yx} & \sigma_{y} & \tau_{yz} \\
\tau_{zx} & \tau_{zy} & \sigma_{z}
\end{bmatrix}
$$
### Spänningar på allmän snittyta
För en godtycklig snittyta $(x,y,z)-$system med normal $\underset{\sim}{n} = (n_{x}, n_{y},n_{z}), \ \ |\underset{\sim}{n}|=1$ så vill vi bestämma spänningsvektorn
$$
\underset{\sim}{s} - \text{Spänningsvektorn}
$$
på snittytan $\underset{\sim}{n}$. Med spänningsmatrisen $\underset{\sim}{S}$ given så blir 
$$
\underset{\sim}{s} = \underset{\sim}{S}^T \cdot \underset{\sim}{n} = \underset{\sim}{S} \cdot \underset{\sim}{n}
$$
där sista sambandet är p.g.a att spänningsmatrisen är symmetrisk. 
### Spänningar 2D
![[Pasted image 20260321091928.png]]
För en snittyta i 2D beräknas normalspänningen och skjuvspänningen enligt
$$
\sigma = \underset{\sim}{n}^T \underset{\sim}{s} = \underset{\sim}{n}^T \underset{\sim}{S} \underset{\sim}{n} 
$$
$$
|\tau|=\sqrt{ |\underset{\sim}{s}|^2-\sigma^2 }
$$

### Huvudspänningar
![[Pasted image 20260321100423.png]]
> [!definition] 
> **Huvudspänning.**
> En huvuspänning är en normalspänning som verkar på en skjuvspänningsfri snittyta. Normalen till en skjuvspänningsfri yta kallas huvudspänningsriktning.

Matematiska kravet är alltså att huvudpänningsvektorn är vinkelrät mot ytan, eller
$$
\underset{\sim}{s}= \underset{\sim}{S} \cdot \underset{\sim}{n}=\sigma \underset{\sim}{n}
$$
för någon skalär $\sigma$. Kravet kan skrivas 
$$
[\underset{\sim}{S}-\sigma I]\underset{\sim}{n} = \underset{\sim}{0}.
$$
där $\underset{\sim}{n}$ är den okända normalspänningsvektorn som vill hittas. Vi har alltså ett egenvärdesproblem med egenvektorer $\underset{\sim}{n_{i}}$ med egenvärden $\sigma_{i}$. I 3D finns alltid tre stycken lösningar $(\sigma_{1}, \sigma_{2}, \sigma_{3})$ och tre huvudspänningsvektorer $(n_{1}, n_{2}, n_{3})$ som är inbördes vinkelräta. Alltså kan varje spänningsmatris diagonaliseras ortogonalt!
### Speciella spänningstillstånd i 3D
- Två huvudspänningar $=0$ $\to$ Enaxlig belastning (t.ex stång)
- En huvudspänning $=0$ $\to$ Plan spänning (t.ex skiva)
- Två huvudspänningar är lika $\to$ Cylindriskt spänningstillstånd.
- Alla tre huvudspänningar like $\to$ Hydrostatiskt eller sfäriskt spänningstillstånd (t.ex vätsketryck).

## Mohrs spänningscirkel

![[Pasted image 20260323130119.png]]












