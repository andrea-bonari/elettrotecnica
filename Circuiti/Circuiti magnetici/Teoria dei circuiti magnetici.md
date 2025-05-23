>[!note]
>È possibile ricavare un equivalente magnetico ai circuiti a parametri concentrati elettrici. In questo caso i flussi $\psi$ sostituiranno le correnti $i$, le riluttanze $\mathcal{R}$ sostituiranno le resistenze $R$, e i generatori di forza elettromotrice $Ni$ sostituiranno i generatori tensione $E$.

>[!example] Dimostrazione
>Consideriamo un anello di materiale ferromagnetico di superficie $\gamma_{1}$. Su esso sono avvolti $N$ avvolgimenti in cui scorre una corrente $i$. Si ha che: $$\Phi(B)=Li$$
>![[Pasted image 20250523100117.png|center]]
>Possiamo quindi ricavare la circuitazione sulla linea $\gamma_{1}$ e $\gamma_{2}$: $$\begin{align*}
>&\oint_{\gamma_{1}}\overrightarrow{H}\cdot \text{d}\overrightarrow{l}=Ni\simeq H_{1}l_{1}\\
>&\oint_{\gamma_{2}}\overrightarrow{H}\cdot\text{d}\overrightarrow{l}=Ni=H_{2}l_{2}
>\end{align*}$$
>Assumendo $H_{1},H_{2}$ costanti e $l_{1},l_{2}$ lunghezze delle linee. Assumiamo: $$l_{1}=l_{2}\Longrightarrow H_{1}l_{1}=H_{2}l_{2}$$
>Abbiamo però che: $$B_{1}=\mu_{0}\mu_{r}H_{1}>>\mu_{0}H_{2}=B_{2}$$
>Possiamo quindi approssimare $\overrightarrow{B}$ a $\overrightarrow{B}_{1}$, cioè la componente interna al materiale ferromagnetico. Proviamo a calcolare quindi $\Phi(\overrightarrow{B})$: $$\psi=\int_{S}\overrightarrow{B}\cdot\hat{u}_{n}\text{ d}S=B_{1}S=\mu_{0}\mu_{r}H_{1}S$$
>Dalla legge di Ampere so che $H_{1}=\frac{Ni}{l_{1}}$, quindi: $$\psi_{1}= \frac{\mu_{r}\mu_{0}NS}{l_{1}}i$$
>Definiamo la riluttanza come: $$\mathcal{R}= \frac{l_{1}}{\mu_{r}\mu_{0}S}\qquad[\mathcal{R}]= \frac{1}{\text{H}}$$
>Abbiamo quindi che: $$\psi= \frac{N}{\mathcal{R}}i\iff \Phi=N\psi= \underbrace{\frac{N^{2}}{\mathcal{R}}}_{L}i$$
>Nel caso più avvolgimenti $i_{1},N_{1}$ e $i_{2},N_{2}$, si ha che: $$\psi=\int_{S}\overrightarrow{B}\cdot\hat{u}_{n}\text{ d}S=BS=\mu_{0}\mu_{r}HS$$
>Usando la legge di Ampere: $$\oint_\gamma\overrightarrow{H}\cdot \text{d}\overrightarrow{l}=N_{1}i_{1}+N_{2}i_{2}=Hl$$
>Abbiamo quindi che: $$H= \frac{N_{1}i_{1}}{l}+ \frac{N_{2}i_{2}}{l}\Longrightarrow \psi= \frac{\mu_{r}\mu_{0}S}{l}N_{1}i_{1}+\frac{\mu_{r}\mu_{0}S}{l}N_{2}i_{2}$$
>Che semplificando: $$\psi= \frac{N_{1}}{\mathcal{R}}i_{1}+ \frac{N_{2}}{\mathcal{R}}i_{2}$$
>Quindi questo oggetto ha matrice di induttanza: $$L=\begin{pmatrix}\frac{N_{1}^{2}}{\mathcal{R}}& \frac{N_{1}N_{2}}{\mathcal{R}}\\ \frac{N_{1}N_{2}}{\mathcal{R}} &\frac{N_{2}^{2}}{\mathcal{R}}\end{pmatrix}$$
>Possiamo da $\psi$ ricavare un equivalente circuitale magnetico ai circuiti a parametri concentrati elettrici, dove al posto di una corrente ho il flusso, al posto della resistenza ho una riluttanza, e al posto dei generatori di tensione ho generatori di forza magnetomotrice.

I circuiti magnetici sono quindi delle reti composte da lati formati da:
- Elementi magneticamente positivi: tratti di materiale ferromagnetici di lunghezza $L_{i}$, sezione $S_{i}$ e permeabilità relativa $\mu_{ri}$. Ha come equivalente elettrico una riluttanza di valore $\mathcal{R}= \frac{L_{i}}{\mu_{ri}\mu_{0}S_{i}}$.
- Elementi magneticamente attivi: tratti di materiale ferromagnetici di lunghezza $L_{k}$, sezione $S_{k}$ e permeabilità $\mu_{rk}$ su cui sono avvolte $N_{k}$ spire percorse da una corrente $i_{k}$. Ha come equivalente elettrico una riluttanza di valore $\mathcal{R}= \frac{L_{k}}{\mu_{rk}\mu_{0}S_{k}}$ in serie ad un generatore di forza magneto motrice di valore $N_{k}i_{k}$.

Definiamo inoltre la tensione magnetica come: $$V_{H}=\mathcal{R}\psi$$
### KCL magnetica
>[!note]
>Dalla legge di Gauss si può ricavare che la somma algebrica dei flussi in una superficie chiusa è nulla: $$\sum\limits_{k}\psi_{k}=0$$

>[!example] Dimostrazione
>Consideriamo una connessione di tratti ferromagnetici su una superficie $\Sigma$. Valgono le leggi di Gauss per il campo $\overrightarrow{B}$: $$\oint_{\Sigma}\overrightarrow{B}\cdot\hat{u}_{n}\text{ d}S=0$$
>Siccome $\overrightarrow{B}$ è interamente contenuto all'interno del materia, si ha che: $$\Sigma=S_{1}+S_{2}+S_{3}+\cdots$$
>Quindi: $$\oint_{\Sigma}\overrightarrow{B}\cdot\hat{u}_{n}\text{ d}S\simeq B_{1}S_{1}+B_{2}S_{2}+B_{3}S_{3}+\cdots=0$$
>
>

### KVL magnetica
>[!note]
>La somma algebrica delle tensioni magnetiche presenti su un percorso chiuso è pari alla somma delle forze elettromotrici.

>[!example] Dimostrazione
>Per la legge di Ampère si ha che: $$\oint_{\gamma}\overrightarrow{H}\cdot \text{d}\overrightarrow{l}=\sum\limits_{i} N_{i}i_{i}$$
>Scomponendo in lati l'integrale possiamo dire: $$\sum\limits_{i} H_{i}L_{i}=\sum\limits_{i} N_{i}i_{i}$$
>Definendo: $$V_{H}= R\psi= \frac{L}{\mu S}\psi= \frac{LBS}{\mu S}= \frac{L\mu HS}{\mu S}=HL$$
>Possiamo dire che: $$\sum\limits_{i}V_{Hi}=\sum\limits_{i}N_{i}i_{i}$$

### Traferro
>[!note]
>Il traferro è un modo per gestire la non linearità dei materiali ferromagnetici.
>![[Pasted image 20250523110057.png|center]]
>Per ipotesi, se $l_{t}<<\sqrt{S}$, allora $\psi$ nel suo traferro è approssimativamente uguale a quello nel ferro. Può essere utilizzato per gestire la non linearità.

>[!example] Dimostrazione
>La riluttanza complessiva è data dalla somma di $\mathcal{R}_{t}$ nel traferro e $\mathcal{R}_{f}$ nel ferro: $$\mathcal{R}=\mathcal{R}_{f}+\mathcal{R}_{t}= \frac{l_{f}}{\mu_{r}\mu_{0}S}+ \frac{L_{t}}{\mu_{0}S}$$
>Se $\mu_{r}>>1$ allora $\mathcal{R}_{t}>>\mathcal{R}_{f}$. Possiamo quindi limitarci a considerare solo la riluttanza nel traferro $\mathcal{R}\simeq\mathcal{R}_{t}$. Quindi l'induttanza complessiva è approssimata a: $$L= \frac{1}{\mathcal{R}}\simeq \frac{\mu_{0}S}{l_{t}}$$
>Andando ad inserire un traferro possiamo eliminare dalle variabili $\mu_{r}$. Assumendo che la sezione $S$ in ferro e traferro rimanga costante: $$\psi_{f}\simeq\psi_{t}\Longrightarrow B_{f}S\simeq B_{t}S\Longrightarrow \mu_{r}\mu_{s}H_{f}\simeq \mu_{0}H_{t}\Longrightarrow H_{z}=\mu_{r}H_{f}$$
>Quindi il campo $H$ nel ferro e traferro è diverso. Approssimo $H$ con la sola componente $H_{t}$. Abbiamo che: $$\oint_{\gamma}\overrightarrow{H}\cdot \text{d}\overrightarrow{l}\simeq H_{t}l_{z}=Ni$$
>Quindi il flusso diventa: $$\psi=BS\simeq \mu_{0}H_{t}S= \frac{\mu_{0}S}{l_{t}}\Longrightarrow\mathcal{R}= \frac{l_{t}}{\mu_{0}S}$$
>Otteniamo che: $$\Phi=N\psi= \frac{N^{2}}{\mathcal{R}_{t}}i$$
