>[!note]
>La tensione è il lavoro necessario per spostare la carica di prova $q$ da un punto $A$ a un punto $B$ lungo la curva $\gamma$ in una regione di spazio in cui è presente un campo elettrico $\overrightarrow{E}$, normalizzato alla carica: $$V_{AB}= \frac{L^{\gamma}_{AB}}{q}=-\int_{\gamma}\overrightarrow{E}\text{ d}\overrightarrow{l}$$
>![[Pasted image 20250218174546.png|center]]

>[!example] Dimostrazione
>Sia $\text{d}L_{1}$ il lavoro necessario per spostare la carica lungo la curva $\gamma$ di una distanza infinitesimale nel generico punto $p_{1}$, allora si calcola come: $$\text{d}L_{1}=q\cdot\overrightarrow{E}_{1}\cos(\theta_{1})=-q\cdot \overrightarrow{E}_{1}\cdot \text{d}\overrightarrow{l}_{1}$$
>![[Pasted image 20250218174534.png|center]]
>
>Dove $\overrightarrow{E}_{1}$ è il valore del campo vettoriale nel generico punto $p_{1}$, e $\theta_{1}$ è l'angolo tra il punto $p_{1}$ e quello successivo nella curva.
>Possiamo approssimare il lavoro su tutta la curva come somma dei lavori infinitesimali: $$L_{AB}^{\gamma}\simeq-q\sum\limits_{k}\overrightarrow{E}_{k}\cdot \text{d}\overrightarrow{l}_{k}$$
>Siccome $\text{d}l_{k}$ è infinitesimale: $$L_{AB}^{\gamma}=-q\int_{\gamma}\overrightarrow{E}\text{ d}\overrightarrow{l}$$
>Normalizzando rispetto alla carica di prova ottengo il valore di tensione tra $A$ e $B$.

### Potenziale elettrico
>[!note]
>Sia $V_{BA}$ la tensione tra i punti $A$ e $B$ lungo un percorso $\gamma$ in una regione di spazio in cui è presente il campo elettrico $\overrightarrow{E}$, si definisce il potenziale elettrico come il valore di energia potenziale normalizzato alla carica: $$q\cdot V_{BA}= q\underbrace{(V(B)-V(A))}_\text{diff. di potenziale}=\underbrace{W(B)-W(A)}_\text{diff. di energia potenziale}$$

>[!example] Dimostrazione
>Sia $\text{d}L_{1}$ il lavoro necessario per spostare la carica lungo la curva $\gamma$ di una distanza infinitesimale nel generico punto $p$.
>
>Scompongo il vettore in una parte parallela al campo elettrico $\text{d}\overrightarrow{l}_{\parallel}$ e una parte perpendicolare $\text{d}\overrightarrow{l}_{\perp}$, quindi: $$\text{d}\overrightarrow{l}=\text{d}\overrightarrow{l}_{\parallel}+\text{d}\overrightarrow{l}_{\perp}$$
>![[Pasted image 20250224142313.png|center]]
>Sappiamo che:$$\text{d}L=-q\cdot \overrightarrow{E}\cdot \text{d}\overrightarrow{l}=- \frac{1}{4\pi\varepsilon_{0}}\cdot \frac{qQ}{||\overrightarrow{r}||^{2}}\hat{r}\cdot \left(\text{d} \overrightarrow{l}_{\parallel}+\text{d}\overrightarrow{l}_{\perp}\right)$$
>Siccome $\hat{r}\cdot \text{d}\overrightarrow{l}_{\perp}=0$, e $\hat{r}\cdot \text{d}\overrightarrow{l}_{\parallel}=||\text{d}\overrightarrow{l}||\cos\theta=||\text{d}\overrightarrow{r}||$: $$\text{d}L= - \frac{qQ}{4\pi\varepsilon_{0}}\cdot \frac{||\text{d}\overrightarrow{r}||}{r^{2}}$$
>Quindi: $$\begin{align*}
>L_{AB}&=  - \frac{qQ}{4\pi\varepsilon_{0}}\int_{A}^{B} \frac{\text{d}r}{r^{2}}=  \frac{qQ}{4\pi\varepsilon_{0}}\cdot \left[\frac{1}{r}\right]^{B}_{A}\\
>&= \frac{qQ}{4\pi\varepsilon_{0}r_{B}}- \frac{qQ}{4\pi\varepsilon_{0}r_{A}}\\
>&= W(B)-W(A)\\
>&= q(V_{B}-V_{A})=q\cdot V_{BA}
>\end{align*}$$
>Dove $W(P)$ è l'energia potenziale di $\overrightarrow{E}$, $V(P)$ potenziale elettrico, e $V_{BA}$ una differenza di potenziale (tensione).

Se il lavoro non dipende dal percorso, allora il campo elettrico $\overrightarrow{E}$ è conservativo. Si dimostra che se $\overrightarrow{E}$ è quasi stazionario, allora è conservativo.

### Legge di Kirchhoff per le tensioni  (KVL)
>[!note]
>Lungo una qualunque linea chiusa, la somma algebrica delle tensioni, prese con il segno opportuno in base al verso di percorrenza della linea, è nulla.

>[!example] Dimostrazione
>Sia $\gamma_{1}$ il percorso che porta da $A$ a $B$, e $\gamma_{2}$ il percorso che porta da $B$ as $A$. Sappiamo che: $$\begin{align*}
>L_{AB}^{\gamma_{1}}&= q(V_{B}-V_{A})\\
>L_{BA}^{\gamma_{2}}&= q(V_{A}-V_{B})
>\end{align*}$$
>![[Pasted image 20250224143432.png|center]]
>Sia quindi $\gamma=\gamma_{1}\cup\gamma_{2}$ il percorso chiuso. Si ha che $L^{\gamma}=L_{AB}^{\gamma_{1}}+L_{BA}^{\gamma_{2}}=0$.
>Per definizione: $$-q\oint_{\gamma}\overrightarrow{E} \text{ d}\overrightarrow{l}=0$$
>Quindi, in regime quasi stazionario, la circuitazione di $\overrightarrow{E}$ è nulla, e di conseguenza la tensione complessiva su una linea chiusa è pari a $0$.

