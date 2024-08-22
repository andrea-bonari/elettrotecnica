>[!note] Lump Circuit Model
>Il Lump Circuit Model è modello per circuiti a parametri concentrati, tuttavia è solo un approssimazione valida soltanto se la lunghezza caratteristica del circuiti è molto inferiore rispetto alla lunghezza d'onda dei segnali presenti sul circuito:
>$$L_{c}<<\lambda \frac{c}{f}$$
>dove $c$ è la velocità della luce e $f$ è la frequenza del segnale.

>[!example]
>Una rete casalinga avrà una frequenza molto bassa:
>$$\lambda= \frac{3\cdot10^{8} \text{m/s}}{60 \text{Hz}}=5\cdot 10^{5}\text{m}$$
>Mentre un microprocessore avrà una frequenza estremamente alta
>$$\lambda= \frac{3\cdot10^{8} \text{m/s}}{3\cdot 10^{9} \text{Hz}}=10\text{cm}$$

### Componenti di un circuito
Per definizione, diciamo che un componente è un modello di un sistema fisico, per esempio un resistore. Diamo un nome alle varie parti di un componente:
![[Pasted image 20240223142412.png]]
<ul style="background-color: #333; margin-top: 0; margin-bottom: 0"><li style="color: yellow">superficie limite</li>
<li style="color: green">morsetto</li>
<li style="color: purple">terminale</li>
<li style="color: cyan">polo (morsetto+terminale)</li></ul>

In base al numero di poli un componente si definisce $n$-polo. Un $n$-polo è definito da una corrente, una tensione e un equazione costitutiva. Possiamo dire, in generale, che per descrivere un $n$-polo sono necessarie $n-1$ correnti, $n - 1$ tensioni e $n-1$ equazioni costitutive.

### Fondamenti di teoria dei grafi
>[!note]
>Un grafo è un insieme di $n$ nodi e $l$ lati. Se i lati sono orientati parliamo di grafo orientato, viceversa se i lati non sono orientati parliamo di grafo non orientato.
>![[Pasted image 20240223143713.png]]

Diamo delle definizioni ai componenti di un grafo:
>[!note] Percorso
>(In giallo nell'immagine) Insieme di lati che collegano due nodi

>[!note] Maglia
>(In verde nell'immagine) Un percorso chiuso

>[!note] Sottografo
>(In viola nell'immagine) Sottoinsieme di nodi e lati

>[!note] Taglio
>(In azzurro nell'immagine) Insieme di lati che, se rimossi, separano il grafo in due sottografi non connessi

>[!note] Grafo connesso
>Grafo dove esiste un percorso che collega qualunque coppia di nodi

>[!note] Albero
>Sottografo aciclico e connesso contenente tutti gli $n$ nodi (e $n-1$ lati)

>[!note] Co-albero
>Insieme di lati non facenti parte dell'albero

### Grafo di un componente
In generale, possiamo associare a ciascun componente un grafo. Il grafo del circuito sarà dato dalla connessione di ogni componente. Possiamo distinguerli in grafi a stella o in grafi non a stella.

##### Grafo a stella
Fissa un nodo di riferimento con cui descrivere il resto del componente
![[Pasted image 20240227150215.png]]
>Il primo grafo indica tutti i dati, Il secondo è orientato come le tensioni mentre il terzo è orientato come le correnti.
##### Grafo non a stella
Non utilizza alcun nodo di riferimento

### Convenzione degli utilizzatori e dei generatori

Le convenzioni sono applicabili solo al caso di grafo a stella
##### Convenzione normale (o degli utilizzatori)
>[!note]
>In ciascun lato associato a un componente le tensioni e le correnti sono prese con verso opposto
>![[Pasted image 20240227150531.png]]

##### Convenzione dei generatori
>[!note]
>In ciascun lato associato a un componente le tensioni e le correnti sono prese con verso concorde.
>![[Pasted image 20240227150555.png]]

---

>[!tip]
>La scelta della convenzione da utilizzare è arbitraria, ma è richiesta coerenza.

>[!example]
>![[Pasted image 20240227151200.png]]
>Utilizzando la convenzione normale si ha $V'=R'i'$, mentre se utilizziamo la convenzione dei generatori abbiamo $V''=-R''i'''$.

In un circuito non è necessario utilizzare la stessa convenzione per tutti i componenti, tuttavia si può passare da un tipo di grafo all'altro soltanto se tutti i componenti rispettano la stessa convenzione
