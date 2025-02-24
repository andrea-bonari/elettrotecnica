>[!note]
>Sia il campo vettoriale $\overrightarrow{A}$ definito su una superficie $S$, dove ad ogni pezzo di superficie $\text{d}S$ un vettore normale $\hat{u}_{n}$:
>![[Pasted image 20250224144608.png]]
>Definisco $\overrightarrow{A}\cdot\hat{u}_{n}\cdot\text{d}S$ come flusso del campo $\overrightarrow{A}$ attraverso una superficie $\text{d}S$.
>Possiamo approssimare il flusso totale come: $$\Phi_{S}(\overrightarrow{A})\simeq\sum\limits_{k}A_{k}\cos\theta_{k}\text{ d}S_{k}$$
>Che per $\text{d}S_{k}\to0$: $$\Phi_{S}(\overrightarrow{A})=\int_{S} \overrightarrow{A}\cdot \hat{u}_{n}\text{ d}S$$

### Legge di Gauss
>[!note]
>Il flusso di un campo elettrico attraverso una superficie chiusa è dato dal rapporto tra la carica elettrica totale interna alla superficie e la costante dielettrica assoluta del mezzo: $$\Phi(\overrightarrow{E})= \frac{Q}{\varepsilon_{0}}$$

>[!example]
>Sia il flusso di $\overrightarrow{E}$ generato da una carica puntiforme $Q$ attraverso una superficie chiusa di forma sferica:
>![[Pasted image 20250224151841.png]]
>Sapendo che: $$\begin{align*}
>\overrightarrow{E}&=  \frac{1}{4\pi\varepsilon_{0}}\cdot \frac{Q}{||\overrightarrow{r}||^{2}}\cdot \hat{r}\\
>\Phi_{S}(\overrightarrow{E})&= \oint_{S}\overrightarrow{E}\cdot \hat{u}_{n}\text{ d}S
>\end{align*}$$
>Allora: $$\Phi_{S}(\overrightarrow{E})= \frac{Q}{4\pi\varepsilon_{0}r^{2}}\oint\underbrace{\hat{r}\cdot \hat{u
>}_{n}}_{1}\text{ d}S= \frac{Q}{\varepsilon_{0}}$$

