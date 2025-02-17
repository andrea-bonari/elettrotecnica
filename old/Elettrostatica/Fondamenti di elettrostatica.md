>[!note]
>L'elettrostatica è una parte dell'elettromagnetismo che studia le cariche elettriche e i campi da esse generate.

### Carica
>[!note]
>La carica è una qualità fondamentale della materia, è una grandezza quantizzata (multiplo della carica elementare).

>[!tip] Carica elementare
>$$q_{e}=-1.6\space ... \cdot 10^{-19}\text{ C}$$

>[!tip] Cariche puntiformi
>Una carica puntiforme è intesa come concentrata in un unico punto del campo.

Da adesso in poi considereremo tutte le cariche puntiformi nel vuoto.

### Legge di Coulomb
>[!note]
>Definiamo il vettore differenza tra due cariche $Q_{1}$ e $Q_{2}$ come $\overrightarrow{r }_{12}=\overrightarrow{r}_{1}-\overrightarrow{r}_{2}$.
>La forza esercitata da $Q_{1}$ su $Q_{2}$ è definita come: $$\overrightarrow{F}_{Q_{1}Q_{2}}= k\frac{Q_{1}Q_{2}}{r^{2}_{21}}\hat{r}_{21}$$
>Dove il coefficiente $k$ equivale a $$k = \frac{1}{4\pi\varepsilon_{0}}\Longrightarrow \overrightarrow{F}_{Q_{1}Q_{2}}= \frac{1}{4\pi\varepsilon_{0}} \cdot \frac{Q_{1}Q_{2}}{r^{2}_{21}}\hat{r}_{21}$$
>e $\varepsilon_{0}$ è la costante dielettrica del vuoto.

>[!tip] Costante dielettrica del vuoto
>$$\varepsilon_{0}=8.85418\space ...\cdot 10^{-12} \frac{\text{F}}{\text{m}}$$

>[!tip] Carica di prova
>La carica di prova è una carica infinitesima positiva:
>$$q>0 \text{ infinitesima}$$
### Campo elettrico
>[!note]
>Un campo elettrico è un campo vettoriale definito operativamente come:
>$$\overrightarrow{E}= \frac{\overrightarrow{F}}{q}$$

>[!tip] Campo
>Il campo è una funzione che associa a un determinato punto dello spazio un determinato valore. Il campo si distingue in campo scalare e campo vettoriale.
>
>Un campo scalare associa a un punto nello spazio ad uno scalare: $$f(x,y,z,t)=\alpha$$
>Un campo vettoriale associa a un punto nello spazio un vettore: $$\overrightarrow{g}(x,y,z,t)=\overrightarrow{v}$$
>
>Le linee di campo sono definite come l'insieme di tutti i punti a cui il campo è tangente:
>![[Pasted image 20240821162658.png]]

Il campo elettrico può essere classificato nei seguenti metodi:

| nome              | condizione                                                         | significato                             |
| ----------------- | ------------------------------------------------------------------ | --------------------------------------- |
| stazionario       | $$\frac{\partial}{\partial t} \overrightarrow{E}(x,y,z,t)=0$$      | non varia nel tempo                     |
| quasi-stazionario | $$\frac{\partial}{\partial t} \overrightarrow{E}(x,y,z,t)\simeq0$$ | varia estremamente lentamente nel tempo |

 Un campo elettrico $\overrightarrow{E}$ generato da una carica puntiforme $Q$ è definito come:
 $$\begin{align*}
&\overrightarrow{F}_{Qq}= \frac{1}{4\pi\varepsilon_{0}}\cdot \frac{Qq}{r^{2}}\hat{r}&\Longrightarrow\\
&\overrightarrow{E}= \frac{\overrightarrow{F}_{Qq}}{q}= \frac{1}{4\pi\varepsilon_{0}}\cdot \frac{Q}{r^{2}}\hat{r}
\end{align*}$$
Il campo elettrico $\overrightarrow{E}$ sarà disposto radialmente.
Se la carica $Q$ è positiva, la direzione del campo elettrico sarà verso l'esterno, viceversa, se $Q$ è negativa, la direzione del campo sarà verso l'interno.

### Tensione elettrica
>[!note]
>La tensione elettrica è il lavoro svolto da un campo elettrico $\overrightarrow{E}$ per spostare una carica normalizzato rispetto ad essa: $$V_{AB}= \frac{L^{\gamma}_{AB}}{q}=-\int_{\gamma}\overrightarrow{E}\cdot\text{d}\overrightarrow{l}$$

>[!example] Dimostrazione
>Poniamo una carica di prova $q$ in una regione di spazio in cui è presente un campo elettrico $\overrightarrow{E}$, il campo $\overrightarrow{E}$ esercita una forza su $q$ e quindi compie un lavoro su $q$. Vogliamo quantificare il lavoro necessario a spostare $q$ in presenza di $\overrightarrow{E}$ da $A$ a $B$ lungo una curva $\gamma$.
>![[Pasted image 20240822123216.png]]
>
>Suddividiamo la curva in piccoli segmenti di modulo infinitesimale:
>![[Pasted image 20240822123301.png]]
>
>Possiamo dire che il lavoro per spostare la carica da $P_{1}$ a $P_{2}$ in opposizione del campo elettrico sarà:
>$$L_{P_{1}P_{2}}\simeq -q E_{1} \cos\theta_{1} \text{d}l_{1}= -q \overrightarrow{E}_{1}\cdot \text{d}\overrightarrow{l}_{1}$$
>Analogamente per spostare da $P_{2}$ a $P_{3}$:
>$$L_{P_{2}P_{3}}\simeq -q E_{2} \cos\theta_{2} \text{d}l_{2}= -q \overrightarrow{E}_{2}\cdot \text{d}\overrightarrow{l}_{2}$$
>E quindi:
>$$L^{\gamma}_{AB}\simeq -q \sum\limits_{k} \overrightarrow{E}_{k}\cdot \text{d} \overrightarrow{l}_{k}$$
>Per $\text{d}\overrightarrow{l}_{k}\to0$:
>$$L^{\gamma}_{AB}=-q \int_{\gamma} \overrightarrow{E}\cdot \text{d}\overrightarrow{l}$$
>Normalizzando il lavoro alla carica:
>$$V_{AB}= \frac{L^{\gamma}_{AB}}{q}=-\int_{\gamma}\overrightarrow{E}\cdot\text{d}\overrightarrow{l}$$
