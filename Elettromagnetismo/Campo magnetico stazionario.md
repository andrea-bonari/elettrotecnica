>[!note]
>Un campo magnetico $\overrightarrow{B}$ è detto stazionario quando: $$\frac{\partial}{\partial t}\overrightarrow{B}(x,y,z,t)=0$$

### Legge di Ampère-Laplace
>[!note]
>Consideriamo il campo magnetico generato da una spira chiusa percorsa da una corrente $I$. Si ha che: $$\overrightarrow{B}= \frac{\mu_{0}I}{4\pi}\oint_{\gamma} \frac{\hat{u}_{t}\times\hat{u}_{r}}{r^{2}}\text{ d}l$$
>![[Pasted image 20250522154706.png|center]]

>[!example] Dimostrazione
>Consideriamo il campo magnetico generato da una spira chiusa percorsa da corrente. Si ha che: $$\text{d}\overrightarrow{B}= \frac{\mu_{0}}{4\pi r^{2}} \Delta Q\cdot \overrightarrow{ v}\times\hat{u}_{r}$$
>Dove $\Delta Q$ è la quantità di carica in un cilindretto di lunghezza $\Delta l$. Abbiamo che: $$\overrightarrow{v}= \frac{\Delta l}{\Delta t}\hat{u}_{t}$$
>E quindi: $$\text{d}\overrightarrow{B}= \frac{\mu_{0}}{4\pi r^{2}} \frac{\Delta Q}{\Delta t} \Delta l\cdot\hat{u}_{t}\times \hat{u}_{r}= \frac{\mu_{0}I}{4\pi r^{2}}\Delta l\cdot \hat{u}_{t}\times\hat{u}_{r}$$
>Per calcolare $\overrightarrow{B}$, prendiamo il caso limite $\lim_{\Delta l\to0}$ e scrivo l'integrale di linea: $$\overrightarrow{B}= \frac{\mu_{0}I}{4\pi}\oint_{\gamma} \frac{\hat{u}_{t}\times\hat{u}_{r}}{r^{2}}\text{ d}l$$

### Legge di Bio-Savart
>[!note]
>Si ha che, per un conduttore di lunghezza infinita: $$\overrightarrow{B}= \frac{\mu_{0}I}{2\pi R}\hat{u}_{\theta}$$

>[!example] Dimostrazione
>Calcoliamo il $\overrightarrow{B}$ generato da una corrente in un conduttore di lunghezza infinita. Sapendo che: $$\begin{align*}
>\overrightarrow{B}&= B\hat{u}_{\theta}\\
>\hat{u}_{t}\times\hat{u}_{r}&= \sin\theta\hat{u}_{\theta}
>\end{align*}$$
>![[Pasted image 20250522154935.png|center]]
>Scrivendo la legge di Ampère-Laplace: $$B= \frac{\mu_{0}I}{4\pi}\int^{+\infty}_{-\infty} \frac{\sin\theta}{r^{2}}\text{ d}l$$
>Sappiamo che $r^{2}=R^{2}+l^{2}$ oppure $R=r\sin(\pi-\theta)=r\sin\theta$. E quindi: $$B= \frac{\mu_{0}I}{4\pi}\int_{-\infty}^{+\infty} \frac{R}{(R^{2}+l^{2})^{\frac{3}{2}}}\text{ d}l$$
>Consideriamo l'integrale: $$\int_{-\infty}^{+\infty} \frac{R}{(R^{2}+l^{2})^{\frac{3}{2}}}\text{ d}l=\int_{0}^{+\infty} \frac{2R}{(R^{2}+l^{2})^{\frac{3}{2}}}\text{ d}l= \frac{2Rl}{R^{2}\sqrt{R^{2}+l^{2}}}\bigg|^{+\infty}_{0}= \frac{2}{R}$$
>E quindi si ha: $$\overrightarrow{B}= \frac{\mu_{0}I}{2\pi R}\hat{u}_{\theta}$$

### Campo magnetico in asse spira circolare
>[!note]
>Si ha che il campo magnetico per una generica spira circolare è definito come: $$\overrightarrow{B}= \frac{\mu_{0}Ia^{2}}{(a^{2}+x^{2})^{\frac{3}{2}}}\hat{u}_{x}$$
>Con $a$ raggio della spira e $x$ distanza del generico punto $P$ dalla spira. Nel centro della spira ha valore: $$B_{C}= \frac{\mu_{0}I}{2a}$$

>[!example] Dimostrazione
>Consideriamo una spira circolare di raggio $a$. Consideriamo un punto generico $P$ distante $r$ da un punto generico $A$ sulla spira. Si ha che: $$\text{d}\overrightarrow{B}= \frac{\mu_{0}}{4\pi}I \frac{\text{d}l}{r^{2}}$$
>![[Pasted image 20250522160411.png|center]]
>Si ha che $\text{d}\overrightarrow{B}=\text{d}\overrightarrow{B}_{\parallel}+\text{d}\overrightarrow{B}_{\perp}$. Per simmetria, importa soltanto $\text{d}B_{\parallel}$. Si ha quindi che: $$\text{d}\overrightarrow{B}_{\parallel}=\text{d}\overrightarrow{B}\cos\alpha$$
>Con $\cos\alpha = \frac{a}{\sqrt{a^{2}+x^{2}}}$. Quindi si ha: $$\overrightarrow{B}=\oint_{\gamma}\text{ d}\overrightarrow{B}_{\parallel}= \frac{\mu_{0}I}{4\pi}\oint \frac{a}{(a^{2}+x^{2})^{\frac{3}{2}}}\text{ d}l= \frac{\mu_{0}I}{4\pi} \frac{a}{(a^{2}+x^{2})^{\frac{3}{2}}}\oint_{\gamma}\text{ d}l= \frac{\mu_{0}Ia^{2}}{(a^{2}+x^{2})^{\frac{3}{2}}}\hat{u}_{x}$$

>[!tip] Solenoide
>Definiamo un solenoide come un avvolgimento di $N$ spire di lunghezza $l$ con: $$\overrightarrow{B}=\mu_{0} \frac{NI}{l}$$
>Realmente un solenoide è un unico avvolgimento di $N$ spire in cui scorre una corrente $I$.
>![[Pasted image 20250522161420.png|center]]

### Legge di Ampère
>[!note]
>Si ha che la circuitazione del campo magnetico $\overrightarrow{B}$ lungo una linea chiusa $L$ è data dalla risultante delle correnti concatenate con $L$: $$\oint_{L}\overrightarrow{B}\cdot \text{d}l=\mu_{0}I$$
>![[Pasted image 20250522161636.png|center]]
>Dalla definizione di $I=\int_{S}\overrightarrow{j}\cdot\hat{u}_{n}\text{ d}S=\Phi_{S}(\overrightarrow{j})$: $$\oint_{L}\overrightarrow{B}\cdot \text{ d}l=\mu_{0}\int_{S}\overrightarrow{J}\cdot\hat{u}_{n}\text{ d}S$$
>Da qui ricaviamo che $\overrightarrow{B}$ è un campo non conservativo, e non è quindi possibile definire un potenziale magnetico.

### Flusso magnetico
>[!note]
>Definiamo il flusso magnetico come: $$\Phi_{B}(\overrightarrow{B})=\int \overrightarrow{B}\cdot\hat{u}_{n}\text{ d}S\qquad[\Phi_{B}]=\text{Wb}=\text{T}\cdot\text{m}^{2}$$
>Si ha che il flusso totale di un campo magneti attraverso una superficie chiusa è sempre nulla (Legge di Gauss per il campo magnetico): $$\oint_{S}\overrightarrow{B}\cdot\hat{u}_{n}\text{ d}S=0= \frac{Q}{\varepsilon_{0}}$$
>Quindi il campo magnetico è solenoidale.

>[!tip] Campi solenoidali
>Si definisce un campo vettoriale solenoidale se: $$\oint_{S}\overrightarrow{A}\cdot\hat{u}_{n}\text{ d}S=0$$

### Leggi di Maxwell per campi elettromagnetici stazionari
>[!note]
>Definiamo le leggi di Maxwell per i campi elettromagnetici stazionari come: $$\begin{align*}
>&\oint_{S}\overrightarrow{E}\cdot\hat{u}_{n}\text{ d}S= \frac{Q}{\varepsilon_{0}}\qquad&\text{Legge di Gauss per il campo elettrico}\\
>&\oint_{S}\overrightarrow{B}\cdot\hat{u}_{n}\text{ d}S= 0\qquad&\text{Legge di Gauss per il campo magnetico}\\
>&\oint_{L}\overrightarrow{E}\cdot \text{d}\overrightarrow{l}= 0\qquad&\text{Circuitazione del campo elettrico (KVL)}\\
>&\oint_{L}\overrightarrow{B}\cdot \text{d}\overrightarrow{l}=\mu_{0}\int_{S}\overrightarrow{j}\cdot\hat{u}_{n}\text{ d}S\qquad&\text{Circuitazione del campo magnetico}
>\end{align*}$$
>Queste leggi valgono se: $$\frac{\text{d}\overrightarrow{E}}{\text{d}t} \simeq0\land\frac{\text{d}\overrightarrow{B}}{\text{d}t}\simeq0$$
