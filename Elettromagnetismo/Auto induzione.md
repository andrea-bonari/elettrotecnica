>[!note]
>SI ha che, in una spira su una curva $\gamma$ in cui scorre una corrente $I$: $$\Phi_{S}(\overrightarrow{B})=\Phi_{\overrightarrow{B}}(I)=I\underbrace{\int_{S} \left( \frac{\mu_{0}}{4\pi}\oint_{\gamma} \frac{\hat{u}_{t}\times\hat{u}_{n}}{r^{2}}\cdot \text{d}\overrightarrow{l}\space\right)\cdot\hat{u}_{n}\text{ d}S}_{L}\qquad [L]= \frac{\text{Wb}}{\text{A}}$$
>Questa è l'equazione costitutiva dell'induttore. $L>0$ è detta auto induttanza del circuito. Se avessimo più di una spira, siamo nel caso di mutua induzione. Nel caso $n=2$, scorrono due correnti $I_{1}$ e $I_{2}$ che generano due campi magnetici $\overrightarrow{B}_{1}$ e $\overrightarrow{B}_{2}$. Nel caso in cui le linee di campo attraversino entrambe le spire avremo che: $$\begin{cases}
>\Phi_{1}=L_{11}I_{1}+L_{12}I_{2} \\
>\Phi_{2}=L_{21}I_{1}+L_{22}I_{2}
>\end{cases}\Longrightarrow L=\begin{pmatrix}L_{11}&L_{12} \\ L_{21}&L_{22}\end{pmatrix}$$
>Dove $L$ è la matrice di induttanza. Generalmente si ha che $L_{12}=L_{21}=L_{M}$ con $L_{M}$ mutua induttanza.

>[!example] Dimostrazione
>Consideriamo una spira su una curva $\gamma$ in cui scorre una corrente $I$, e consideriamo il campo magnetico da essa generato come usando la legge di Ampère-Laplace: $$\overrightarrow{B}= \frac{\mu_{0}I}{4\pi}\oint_{\gamma} \frac{\hat{u}_{t}\times\hat{u}_{n}}{r^{2}}\cdot\text{d}\overrightarrow{l}$$
>Consideriamo il flusso autoconcatenato di $\overrightarrow{B}$: $$\Phi_{S}(\overrightarrow{B})=\int_{S} \left( \frac{\mu_{0}I}{4\pi}\oint_{\gamma} \frac{\hat{u}_{t}\times\hat{u}_{n}}{r^{2}}\cdot \text{d}\overrightarrow{l}\space\right)\cdot\hat{u}_{n}\text{ d}S$$
>Possiamo estrarre la corrente $I$ e fare in modo che: $$\Phi_{S}(\overrightarrow{B})=\Phi_{\overrightarrow{B}}(I)=I\underbrace{\int_{S} \left( \frac{\mu_{0}}{4\pi}\oint_{\gamma} \frac{\hat{u}_{t}\times\hat{u}_{n}}{r^{2}}\cdot \text{d}\overrightarrow{l}\space\right)\cdot\hat{u}_{n}\text{ d}S}_{L}$$
>Questa è l'equazione costitutiva dell'induttore. $L>0$ è detta auto induttanza del circuito.

>[!tip] Flusso autoconcatenato
>Definiamo il flusso autoconcatenato come il flusso di $\overrightarrow{B}$ attraverso una superficie $S$: $$\Phi_{S}(\overrightarrow{B})=\int_{S}\overrightarrow{B}\cdot\hat{u}_{n}\text{ d}S$$

