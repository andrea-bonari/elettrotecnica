>[!note]
>L'elettrostatica è la parte dell'elettromagnetismo che studia le cariche elettriche e i campi elettrici da essi generati.

### Carica

La carica è una qualità fondamentale della materia, ed è detta quantizzata perché può assumere solo valori multipli di un valore fondamentale detto carica fondamentale dell'elettrone, cioè $$q_{e}=1.6\dotsc \cdot10^{-19} \text{ C}$$

>[!tip] Cariche puntiformi
>Le cariche puntiformi sono cariche intese come concentrate in un singolo punto dello spazio nel vuoto.

### Legge di Coulomb
>[!note]
>La legge di Coulomb studia l'interazione fra le cariche puntiformi, nel senso che misura la forza esercitata da una carica $Q_{1}$ su una carica $Q_{2}$
>
>$$\overrightarrow{F_{Q_{1}Q_{2}}}=k\cdot\frac{Q_{1}\cdot Q_{2}}{||\overrightarrow{r_{2}r_{1}}||^{2}}\cdot \widehat{r_{2}r_{1}}\Rightarrow k= \frac{1}{4\pi\epsilon_{0}}\Rightarrow F_{Q_{1}Q_{2}}= \frac{1}{4\pi\epsilon_{0}}\cdot \frac{Q_{1}\cdot Q_{2}}{||\overrightarrow{r_{2}r_{1}}||^{2}}\cdot \widehat{r_{2}r_{1}}$$

>[!tip] Costante dielettrica del vuoto
>La costante dielettrica del vuoto $\epsilon_{0}$ è pari a $$\epsilon_{0}=8.85418\dotsc\cdot10^{-12} \frac{F}{m}$$

Possiamo notare che, essendo la distanza tra due cariche $\overrightarrow{r_{2}r_{1}}=\overrightarrow{r_{2}}-\overrightarrow{r_{1}}$, esse si attraggono se hanno segno discorde, e analogamente, si respingono se hanno segno concorde.
![[Pasted image 20240220160011.png]]

### Campo elettrico
>[!note]
>Un campo è una funzione continua che associa ad un punto dello spazio un particolare valore (in un dato tempo).
>
>Può essere distinto in due tipologie:
>- Campo scalare: $$f(\underbrace{x,y,z}_\text{punto},\underbrace{t}_\text{tempo})=\underbrace{a}_\text{scalare}$$
>- Campo vettoriale: $$f(\underbrace{x,y,z}_\text{punto},\underbrace{t}_\text{tempo})=\underbrace{\overrightarrow{v}}_\text{vettore}$$

Le linee di campo sono l'insieme dei punti a cui un dato campo vettoriale è tangente. Un visualizzazione fisica di un campo può essere.
![[Pasted image 20240220160614.png]]

>[!tip] Carica di prova
>Sia $q>0$ una carica infinitesima positiva, allora può essere considerata carica di prova se:
>- La carica è soggetta alla forza generata dalle altre cariche
>- La carica non perturba (per approssimazione) il campo elettrico.

>[!note] Campo Elettrico
>La definizione operativa di campo elettrico è $$\overrightarrow{E}= \frac{\overrightarrow{F}}{q}$$
>Inoltre il campo elettrico si dice:
>- Stazionario se non cambia nel tempo: $$\frac{d}{dt}\overrightarrow{E}(x,y,z,t)=0$$
>- Quasi stazionario se varia nel tempo molto lentamente rispetto alle variazioni interne al circuito $$\frac{d}{dt}\overrightarrow{E}(x,y,z,t)\simeq0$$


Per la legge di Coulomb vale $$\overrightarrow{E}=\frac{\overrightarrow{F}}{q}=\frac{1}{4\pi\epsilon_{0}}\cdot\frac{Q_{1}}{d^{2}}\widehat{r}\qquad,\quad d=|\overrightarrow{r}|$$
Quindi il campo elettrico generato da una carica multiforme è disposto radialmente e se:
- carica positiva => uscente
- carica negativa => entrante

