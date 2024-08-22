### Tensione elettrica

Poniamo una carica di prova in una regione di spazio in cui è presente il campo elettrico $\overrightarrow{E}$, la carica di prova si sposterà lungo le linee di campo del campo elettrico $\overrightarrow{E}$, questo perché compie un lavoro sulla carica di prova $q$. Supponiamo di voler calcolare il lavoro necessario per spostare la carica di prova $q$ in presenza del campo elettrico $\overrightarrow{E}$, quindi vogliamo spostare $q$ da $A$ a $B$ lungo $\gamma$. Consideriamo delle spezzate abbastanza piccole da approssimare la curva $\gamma$.
![[Pasted image 20240220162026.png]]

Possiamo dire che il lavoro necessario per spostare $q$ da $P_{1}$ a $P_{2}$ è: $$L_{P_{1}P_{2}}\simeq -q\cdot E_{1}\cdot\cos\theta_{1}\cdot dl_{1}=-q\overrightarrow{E_{1}}\cdot d\overrightarrow{l_{1}}$$
analogamente per calcolare il lavoro per spostare $q$ da $P_{2}$ a $P_{3}$:
$$L_{P_{2}P_{3}}\simeq -q\cdot E_{2}\cdot\cos\theta_{2}\cdot dl_{2}=-q\overrightarrow{E_{2}}\cdot d\overrightarrow{l_{2}}$$
Possiamo ricavare la formula generale
$$L^{\gamma}_{AB}=-q\sum\limits_{k}\overrightarrow{E}_{k}\cdot d\cdot\overrightarrow{l_{k}}$$

>[!tip]
>Il segno meno è da interpretare come lavoro in opposizione al campo elettrico, dato che questo lavoro è compiuto da noi, non dal campo.

vale: $$d\overrightarrow{l_{k}}\to 0: L^{\gamma}_{AB}=-q\int_{\gamma}\overrightarrow{E}\cdot d\overrightarrow{l}$$
>[!tip]
>La tensione elettrica è definita come $$V_{AB}=\frac{L^{\gamma}_{AB}}{q}=-\int_{\gamma}\overrightarrow{E}\cdot d\overrightarrow{l}$$quindi il lavoro è normalizzato alla carica.

### Legge di Kirchhoff per le tensioni (KVL)
>[!note]
>Lungo una qualunque linea chiusa, la somma algebrica delle tensioni, prese con il segno opportuno in base al verso di percorrenza della linea, è nulla. Vale quindi la relazione $$\oint_{\gamma}\overrightarrow{E}\cdot \text{d}\overrightarrow{l}=0$$

>[!example]
>
>Supponiamo di avere una curva $\gamma$ qualsiasi
>![[Pasted image 20240222195159.png]]
>Possiamo dire che $V_{BA}+V_{CB}+V_{AC}=0$, oppure se definiamo al contrario la tensione tra $C$ e $B$ ($V_{BC}$), possiamo dire che $V_{AB}-V_{BC}+V_{AC}=0$

>[!abstract] Dimostrazione
>![[Pasted image 20240222195213.png]]
>Supponiamo di descrivere il vettore $d\overrightarrow{l}$ utilizzando due vettori, uno parallelo al campo elettrico $\overrightarrow{E}$ ($d\overrightarrow{l}_{||}$) e uno perpendicolare allo stesso campo elettrico ($d\overrightarrow{l}_{\perp}$). Allora possiamo dire che $$d\overrightarrow{l} =d\overrightarrow{l}_{||}+d\overrightarrow{l}_{\perp}$$
>Sapendo che $dL=-q\overrightarrow{E}\cdot d\overrightarrow{l}$ sostituiamo la precedente formula e la legge di Coulomb: $$dL=- \frac{1}{4\pi\epsilon_{0}}\cdot \frac{qQ}{r^{2}}\hat{r}\cdot(d\overrightarrow{l}_{||}+d\overrightarrow{l}_{\perp})$$
>Definiamo: $$\hat{r}\cdot d\overrightarrow{l}_{||}+\hat{r}\cdot d\overrightarrow{l}_{\perp}=\hat{r}\cdot d\overrightarrow{l}_{\perp}=dl\cos\theta=dr$$
>E quindi: $$dL=- \frac{qQ}{4\pi\epsilon_{0}}\cdot \frac{dr}{r^{2}}$$
>
>A questo punto se calcoliamo il lavoro per spostare da un punto $A$ a un punto $B$
>$$\begin{align*}L_{AB}&=& \frac{qQ}{4\pi\epsilon_{0}}\int^{B}_{A}- \frac{dr}{r^{2}}= \frac{qQ}{4\pi\epsilon_{0}}\cdot \left[\frac{1}{r}\right]^{B}_{A}=\\&=& \frac{qQ}{4\pi\epsilon_{0}r_{B}}-\frac{qQ}{4\pi\epsilon_{0}r_{A}}=W(B)-W(A)=q(V_{B}-V_{A})=qV_{BA}\end{align*}$$
>
>Possiamo quindi definire $W(P)$ come l'energia potenziale, $V(P)$ come il potenziale elettrico e $V_{P_{1}P_{2}}$ come la differenza di potenziale.
>
>Dall'equazione possiamo definire quindi la tensione come $$V_{AB}= \frac{L^{\gamma}_{AB}}{q}$$
>
>Se il lavoro non dipende dal percorso ma solo dagli estremi, allora il campo è detto conservativo. (NB: un campo $\overrightarrow{E}$ quasi-stazionario è sempre conservativo).
>
>Estendiamo questa dimostrazione anche al caso dei campi quasi stazionari. Consideriamo i due percorsi da $A$ a $B$:
>![[Pasted image 20240222195407.png]]
>Allora i lavori rispettivi saranno $$L^{\gamma_{1}}_{AB}=q(V_{B}-V_{A})\qquad L^{\gamma_{2}}_{BA}=q(V_{A}-V_{B})$$
>
>Consideriamo il percorso $\gamma=\gamma_{1}+\gamma_{2}$, allora il suo lavoro sarà $$L^{\gamma}=L^{\gamma_{1}}_{AB}+L^{\gamma_{2}}_{BA}=0$$
>Quindi l'integrale di line, su una linea chiusa (detto circuitazione) è: $$-\oint_{\gamma}\overrightarrow{E}\cdot d\overrightarrow{l}=0$$

### Flusso di un campo vettoriale
>[!note]
>A una curva $\gamma$ possiamo associare una superficie $S$ da essa limitata.
>Definiamo flusso di un campo $\overrightarrow{A}$ attraverso la superficie $dS$ come $\overrightarrow{A}\cdot \hat{u}_{n} dS$
>![[Pasted image 20240222200059.png]]
>
>Questo flusso può essere approssimato come $\Phi_{S}(\overrightarrow{A})=\sum\limits_{k}A_{k}\cos\theta_{k}dS_{k}$.
>
>Dove $A_{k}$ significa che ogni piccolo quadratino il campo elettrico può essere assunto come costante. Per $dS_{k}\to 0$, allora: $$\Phi(\overrightarrow{A})=\int_{S}\overrightarrow{A}\cdot \overrightarrow{u}_{n}dS$$

Calcoliamo il flusso di $\overrightarrow{E}$ generato da una carica puntiforme attraverso una superficie di forma sferica. Definiamo il raggio come $|\overrightarrow{r}|=r$
![[Pasted image 20240222200642.png]]

Ricordando che $\overrightarrow{E}= \frac{1}{4\pi\epsilon_{0}}\cdot \frac{Q}{r^{2}}\hat{r}$:
$$\Phi(\overrightarrow{E})=\oint_{S}\overrightarrow{E}\cdot \hat{u}_{n}dS=\oint_{S} \frac{1}{4\pi\epsilon_{0}} \frac{Q}{r^{2}}\hat{r}\cdot \hat{u}_{n}dS$$
Calcolando, e ricordando che $\hat{r}$ e $\hat{u}_{n}$ sono paralleli e versori: $$\Phi(\overrightarrow{E})= \frac{Q}{4\pi\epsilon_{0}r^{2}}\cdot 4\pi r^{2}= \frac{Q}{\epsilon_{0}}$$
Possiamo definire questa equazione come legge di Gauss

>[!note] Legge di Gauss per il flusso del campo elettrico
>$$\Phi_{S}(\overrightarrow{E})= \frac{Q}{\epsilon_{0}}$$
>
>Questa legge è valida per qualsiasi superficie in cui sono racchiuse le cariche.

### Corrente elettrica
>[!note]
>La corrente elettrica è la quantità di carica che attraversa la superficie $S$ in un intervallo di tempo $\triangle t$: $$I= \frac{\triangle Q}{\triangle t}\qquad [I]= \left[\frac{C}{s}\right]=A$$
>Per calcolare la corrente istantanea ($\triangle t\to 0$) calcoliamo la derivata per la variabile $t$ $$I=\lim_{\triangle t\to 0}\frac{\triangle Q}{\triangle t}= \frac{dQ}{dt}$$
>
>Ricordiamo che nonostante alla corrente sia associato un verso è comunque un valore scalare.


Diamo una definizione di corrente più rigorosa:
![[Pasted image 20240222212446.png]]

Calcoliamo quanta carica attraversa $S$ in un intervallo di tempo $\triangle t$
$$\triangle Q=v\triangle t\cos\theta\cdot S\cdot \underbrace{\rho_{v}}_\text{densità volumetrica di carica}=\rho_{v}\overrightarrow{v}\cdot\hat{u}_{n}\cdot S\cdot \triangle t$$
Da questa equazione ricaviamo: $$I= \frac{\triangle Q}{\triangle t}=\rho_{v}\overrightarrow{v}\cdot \hat{u}_{n}\cdot S$$
>[!warning]
>$\rho_{v}$ può essere sia negativa che positiva

Indichiamo $\rho_{v}\overrightarrow{v}$ con $\overrightarrow{j}$. Questa variabile è detta campo densità di corrente. Infine diciamo $$I=\Phi_{S}(\overrightarrow{j})=\int_{S}\overrightarrow{j}\cdot \hat{u}_{n}\text{dS}\qquad[\overrightarrow{j}]= \left[\frac{A}{m^{2}}\right]$$
### Materiali conduttori
>[!note]
>Un materiale conduttore è un materiale in cui le cariche sono libere in muoversi, infatti generalmente portano una carica di elettroni. È importante capire 2 cose:
>- Siccome gli elettroni si muovono in modo casuale, in media $I=0$
>- Applicando un campo elettrico la forza a cui saranno soggetti gli elettroni sarà $\overrightarrow{F}=-e\overrightarrow{E}$ dove $-e$ è la carica dell'elettrone. Gli elettroni si muovono con una velocità $\overrightarrow{v}$ in un moto lineare **non** uniformemente accellerato.
>  
>  Sperimentalmente possiamo misurare che $$\overrightarrow{v}=-\mu\overrightarrow{E}$$dove $\mu$ è la mobilità delle cariche libere.

### Legge di Ohm
Supponiamo che:
- i portatori di carica siano elettroni, e quindi $\rho_{v}<0$
- $\overrightarrow{E}$ sia costante all'interno del conduttore.

Definiamo $v\triangle t=\triangle l$ come spazio che la carica percorre in un intervallo di tempo.
![[Pasted image 20240222215043.png]]
##### Calcoliamo la differenza di potenziale tra gli estremi
$$V_{AB}=V_{A}-V_{B}=-\int_{\gamma}\overrightarrow{E}\cdot d\overrightarrow{l}=-E\int_{\gamma}\hat{E}\cdot d\overrightarrow{l}=E\triangle l$$
$$\Rightarrow \quad E= \frac{V_{AB}}{\triangle l}$$

##### Calcoliamo la quantità di carica che attraversa $\triangle S$ in $\triangle t$

$$\triangle Q=\rho_{v}v\triangle t\triangle S=\rho_{v}\mu E\triangle t\triangle S$$
$$\Rightarrow\quad \frac{\triangle Q}{\triangle t}=I=\rho_{v}\mu\frac{V_{AB}}{\triangle l}\triangle S$$

Possiamo quindi enunciare:
>[!note] Leggi di Ohm
>$$I=\underbrace{\gamma}_\text{costante di conduttività} \frac{\triangle S}{\triangle l}V_{AB}= \underbrace{G}_\text{conduttanza}V_{AB}$$
>$$V_{AB}=\underbrace{\rho}_\text{resistività}\frac{\triangle l}{\triangle S}I=\underbrace{R}_\text{resistenza}I$$
>
>Definiamo le unità di misura come:
>$$S=\frac{1}{\ohm}\quad [\gamma]= \frac{S}{M}\quad [G]=S\quad [\rho]=\ohm\cdot m\quad [R]=\ohm$$

>[!abstract]
>Facciamo una piccola precisazione sul verso della corrente: a discapito che noi lavoriamo con cariche negative o positive la direzione di $\overrightarrow{j}$ sarà sempre la stessa di $\overrightarrow{E}$.

### Principio di conservazione della carica
>[!note]
>Sia $S$ una superficie chiusa immersa in un campo elettrico $\overrightarrow{E}$. Abbiamo che: 
>![[Pasted image 20240227064303.png]]
>$$\Phi_{S}(\overrightarrow{j})=\oint_{S}\overrightarrow{j}\cdot\hat{u_{n}}dS=I=- \frac{dQ}{dt}$$
>Il segno meno nel termine $- \frac{dQ}{dt}$ è posto poiché nelle superficie possono entrare o Elettroni ($Q <0$) o uscire ioni positivi ($Q>0$), in entrambi i casi la carica della superficie diminuisce.
>
>Sostituendo la legge di Gauss troviamo la formula:
>$$\oint_{S}\overrightarrow{j}\cdot\hat{u_{n}}dS+ \epsilon_{0} \frac{d}{dt}\oint_{S}\overrightarrow{E}\cdot\hat{u_{n}}dS=0$$
>
>Di conseguenza la presenza di un campo elettrico $\overrightarrow{E}$ variante nel tempo induce una corrente all'interno del materiale conduttore. Possiamo quindi dire che un campo elettrico quasi stazionario avrà il flusso $\overrightarrow{j}$ nullo

### Legge di Kirchhoff per le correnti
>[!note]
>In un regime stazionario o quasi stazionario il bilancio delle correnti entranti e delle correnti uscenti in una superficie chiusa è nullo.
>![[Pasted image 20240227065130.png]]





