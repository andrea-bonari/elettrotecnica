>[!note]
>![[Pasted image 20240822134818.png]]
>Dato $\hat{u}_{n}$ versore normale alla superficie, definisco $\overrightarrow{A}\cdot \hat{u}_{n}\cdot\text{d}S$ come flusso del campo $\overrightarrow{A}$ attraverso la superficie $\text{d}S$. In concetti più semplici si può definire il flusso con quanto volume attraversa la superficie in un unità di tempo.

>[!example]
>![[Pasted image 20240822135405.png]]
>Nella prima figura il flusso è $vS$, nella seconda è pari a 0, mentre nella terza è pari a $v\cos\theta\cdot S=\overrightarrow{v}\cdot \hat{u}_{n}\cdot S$.

Quindi il flusso complessivo del campo vettoriale $\overrightarrow{A}$:
$$\Phi_{S}(\overrightarrow{A})\simeq\sum\limits_{k} A_{k}\cos\theta_{k}\cdot \text{d}S_{k}$$
Che per $\text{d}S_{k}\to0$: $$\Phi_{S}(\overrightarrow{A})=\int_{S} \overrightarrow{A}\cdot \hat{u}_{n}\cdot \text{d}S$$
>[!example]
>Trovare il flusso di $\overrightarrow{E}$ generato da una carica puntiforme $Q$ attraverso una superficie chiusa di forma sferica $S$:
>![[Pasted image 20240822164548.png]]
>$$\overrightarrow{E}= \frac{1}{4\pi\varepsilon_{0}}\cdot \frac{Q}{r^{2}}\hat{r}$$
>$$\begin{align*}
\Phi_{s}(\overrightarrow{E})&=\oint_{S} \overrightarrow{E}\cdot \hat{u}_{n}\cdot \text{d}S\\
&= \frac{Q}{4\pi\varepsilon_{0}r^{2}}\oint_{S}\hat{r}\cdot\hat{u}_{n}\cdot \text{d}S\\
&=  \frac{4Q\pi r^{2}}{4\pi\varepsilon_{0}r^{2}}= \frac{Q}{\varepsilon_{0}}
\end{align*}$$

### Corrente elettrica
>[!note]
>Definiamo la corrente elettrica come variazione di carica:
>$$I= \frac{\Delta Q}{\Delta t}$$
>Per $\Delta t\to0$: $$I= \frac{\text{d}Q}{\text{d}t}$$
>È una quantità scalare, e la sua unità di misura sono $[Cs^{-1}]=[A]$.

>[!example] Dimostrazione
>![[Pasted image 20240822170126.png]]
>Calcoliamo la quantità di carica che si trova nelle superficie $S$.
>$$\begin{align*}
\Delta Q&= v\cdot \Delta t\cdot \cos\theta \cdot S\cdot \underbrace{\rho_{v}}_{\text{densità volumetrica di carica}}\\
&= \rho_{v}\overrightarrow{v}\cdot\hat{u}_{n}\cdot S\cdot \Delta t\\
&\Longrightarrow I= \frac{\Delta Q}{\Delta t}=\rho_{v}\overrightarrow{v}\cdot \hat{u}_{n}\cdot S\\
I &= \Phi_{S}(\overrightarrow{J})=\int_{S}\overrightarrow{J}\cdot \hat{u}_{n}\cdot \text{d}s 
\end{align*}$$ 
 
