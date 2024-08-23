>[!note]
>La teoria dei circuiti è usata per analizzare circuiti a parametri concentrati, cioè un modello ideale dove la propagazione istantanea. È un approssimazione valida a condizione che $$\underbrace{L_{c}}_\text{lunghezza caratteristica del circuito}<<\underbrace{\lambda}_\text{lunghezza d'onda dei segnali presenti nel circuito}= \frac{c}{f}$$
>Dove $c$ è la velocità della luce e $f$ è la frequenza del circuito.

### Componente di un circuito
>[!note]
>Un componente è un modello di un sistema fisico. A ogni componente sono associate delle equazione costitutive che legano variabili descrittive come tensioni e correnti.

>[!tip] Rappresentazione di componenti circuitali
>![[Pasted image 20240822191350.png]]
>><span style="color: yellow;">■</span> superficie limite
>><span style="color: lightgreen;">■</span> morsetto
>><span style="color: pink;">■</span> terminale
>><span style="color: aqua;">■</span> polo (morsetto + terminale)
>
>I componenti si classificano in base al numero di poli e sono detti $n$-poli. Consideriamo componenti con almeno $2$ poli.

In generale un $n$-polo necessita di $n-1$ tensioni, $n-1$ correnti e $n-1$ equazioni costitutive.

### Fondamenti di teoria dei grafi
>[!note]
>Un grafo è un insieme di nodi e lati. Un grafo può essere orientato o non orientato.

>[!example]
>![[Pasted image 20240823101524.png]]
>><span style="color: yellow;">■</span> Percorso: insieme di lati che collega 2 nodi
>><span style="color: lightgreen;">■</span> Maglia: percorso chiuso
>><span style="color: pink;">■</span> Sottografo: un sottoinsieme di nodi e lati
>><span style="color: aqua;">■</span> Taglio: insieme di lati che, se rimossi, separa il grafo in due sottografi non connessi

### Grafo di un componente
>[!note]
>Ad ogni componente è associato un grafo. Il grafo complessivo del circuito sarà dato dall'unione dei singoli grafi.

>[!tip] Grafo a stella
>Usiamo un nodo di riferimento.
>![[Pasted image 20240823102055.png]]

>[!tip] Grafo non a stella
>Non abbiamo un nodo di riferimento.
>![[Pasted image 20240823102219.png]]



