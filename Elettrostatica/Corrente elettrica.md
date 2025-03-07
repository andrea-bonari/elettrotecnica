>[!note]
>Definiamo la corrente elettrica come una variazione di carica: $$\langle I\rangle =\frac{\Delta Q}{\Delta t}\qquad[I]=\text{A}= \frac{\text{C}}{\text{s}}$$
>Per una variazione di tempo infinitesimale: $$I= \frac{\text{d}}{\text{d}t} Q$$

![[Pasted image 20240822170126.png]]
Formalmente per calcolare la quantità di carica che attraversa $S$ nel tempo $\Delta t$: $$\Delta Q=\rho_{v}\cdot v\cdot \Delta t\cdot\cos\theta\cdot S=\rho_{v}\cdot \overrightarrow{v}\cdot \hat{u}_{n}S\Delta t$$Dove $\rho_{v}$ è la densità volumetrica di carica ($[\rho_{v}]= \frac{C}{m^{3}}$). E quindi: $$\begin{align*}
I&=  \frac{\Delta Q}{\Delta t}=\underbrace{\rho_{v}\cdot \overrightarrow{v}}_\text{Campo di densità di corrente}\cdot\hat{u}_{n}\cdot S\\
&= \Phi_{S}(\overrightarrow{J})=\int_{S}\overrightarrow{J}\cdot\hat{u}_{n}\text{ d}S
\end{align*}$$

### Materiale conduttore
>[!note]
>Un materiale conduttore è un materiale in cui le cariche siano libere di muoversi.
>![[Pasted image 20250224154327.png|center]]
>In assenza di $\overrightarrow{E}$ la direzione di attraversamento della superficie $S$ è casuale (in media $I=0$). Applicando $\overrightarrow{E}$, gli elettroni saranno soggetti a una forza $-e\overrightarrow{E}$, e cominceranno all'interno del conduttore ad una velocità $\overrightarrow{v}$, detta di drift. Questo valore è proporzionale al campo elettrico: $$\overrightarrow{v}=-\mu\overrightarrow{E}$$
>Con $\mu$ mobilità delle cariche libere dipendente dal materiale.

### Legge di Ohm
>[!note]
>La legge di Ohm mette in relazione tensione e corrente con la formula: $$V=RI$$
>Dove $R$ è la resistenza, e dipende sia dalle caratteristiche fisiche del materiale, sia dalla sua geometria.

>[!example] Dimostrazione
>![[Pasted image 20240822173135.png|center]]
>Supponiamo per ipotesi che i portatori di carica siano elettroni ($\rho_{v}<0$) e che il campo elettrico $\overrightarrow{E}$ sia costante all'interno del materiale.
>Calcoliamo la differenza di potenziale tra $A$ e $B$:
>$$\begin{align*}
>V_{AB}&=V_{A}-V_{B}=-\int_{\gamma}\overrightarrow{E}\cdot \text{d}\overrightarrow{l}=-E\int_{\gamma}\hat{E}\cdot \text{d}\overrightarrow{l}\\
>&= E\cdot \Delta l\Longrightarrow E= \frac{V_{AB}}{\Delta l}\end{align*}$$
>Calcoliamo la quantità di carica che attraversa $\Delta S$ in $\Delta t$: $$\begin{align*}
>\Delta Q=&\space\rho_{v}\cdot v\cdot\Delta t\cdot\Delta S=\rho_{v}\cdot \mu E\cdot\Delta t\cdot\Delta S\\
>\Longrightarrow&\space I = \frac{\Delta Q}{\Delta t}=\rho_{r}\cdot\mu \cdot \frac{V_{AB}}{\Delta l}\Delta S
>\end{align*}$$
>Riscriviamo $I$ come: $$\begin{align*}
>I&= \gamma \cdot \frac{\Delta S}{\Delta l}\cdot V_{AB}= G\cdot  V_{AB}\\
>V_{AB}&= \rho\cdot \frac{\Delta l}{\Delta S}\cdot I=R\cdot I
>\end{align*}$$
>Con $\gamma$ conduttività ($[\gamma]= \frac{\text{S}}{\text{m}}$), $G$ conduttanza ($[G]=\text{S}$), $\rho$ resistività ($[\rho]=\ohm\cdot \text{m}$) e $R$ resistenza $([R]=\ohm)$.
