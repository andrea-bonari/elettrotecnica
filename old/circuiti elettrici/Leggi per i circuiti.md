### Leggi di Kirchhoff per i circuiti
>[!note] KVL-I
>Dato un circuito che opera in regime stazionario, con $n$ nodi e il cui grafo sia connesso, prendiamo uno dei suoi nodi come riferimento $u_{0}$ per misurare il potenziale elettrico e indichiamo con $u_{1},\cdots,u_{n-1}$ i rimanenti potenziali del nodo. Ad ogni istante di tempo $t$, la tensione $V_{kj}$ misurata tra il nodo $k$ e il nodo $j$ è pari a $u_{k}-u_{j}$

>[!note] KVL-II
>Dato un circuito che opera in regime stazionario, con $n$ nodi e il cui grafo sia connesso, preso un percorso chiuso che passi per $m$ nodi del grafo (ad ogni istante di tempo $t$), la somma algebrica delle tensioni fra i nodi consecutivi che si incontrano lungo il percorso è nulla. La somma si intende algebrica poiché le tensioni che si incontrano lungo il percorso e che sono orientate come il verso di percorrenza del percorso stesso vengono prese con il segno $+$, viceversa quelle orientate nel senso opposto vengono prese con il segno $-$.

>[!note] KCL
>Dato un circuito che opera in regime stazionario, con $n$ nodi e il cui grafo sia connesso, prendiamo una superficie chiusa orientata che tagli solo lati del grafo. In ogni istante di tempo $t$, la somma algebrica di tutte le correnti uscenti e entranti dalla superficie orientata sopra definita è nulla.

>[!tip]
>1. A un circuito con $l$ lati corrispondono $2l$ incognite
>2. "Risolvere un circuito" significa ricavare tutte le incognite
>3. Dobbiamo quindi scrivere un sistema lineare di $2l$ equazioni, dove $l$ equazioni sono le equazioni costitutive mentre $l$ equazioni derivano dalla topologia del circuito (tramite KVL e KCL)
>$$\begin{cases}
l-n+1&KVL-II\\
n-1&KCL
\end{cases}$$
### Matrice di incidenza
>[!note]
>La matrice di incidenza ci permette di rappresentare un grafo in forma compatta, ma soprattutto ci permette di definire una metodologia per scrivere le $l$ equazioni topologiche linearmente indipendenti. La matrice di incidenza è $n\times l$.
>
>La matrice è data da: $$(a_{ij})=\begin{cases}+1&\text{se il lato }j\text{ incide nel nodo }i\text{ ed è uscente}\\-1&\text{se il lato }j\text{ incide nel nodo }i\text{ ed è entrante}\\0&\text{se il lato }j\text{ non incide nel nodo }i\end{cases}$$
>
>Le $n$ righe della matrice $A_{a}$ sono linearmente indipendenti
>
>Rimuovendo una riga dalla matrice, ottengo la matrice ridotta $A$.
>
>Per trovare le $n-1$ KCL calcolo: $$A \overrightarrow{i} = \overrightarrow{0}\qquad\qquad \overrightarrow{i}=\begin{pmatrix}i_{1}\\i_{2}\\\vdots\\i_{l}\end{pmatrix}$$
>
>Per trovare le $l-n+1$ KVL-I calcolo: $$A^{T}\overrightarrow{u}=\overrightarrow{V}\qquad\qquad \overrightarrow{u}=\begin{pmatrix}u_{1}\\u_{2}\\\vdots\\u_{n-1}\end{pmatrix}\quad \overrightarrow{V}=\begin{pmatrix}V_{a}\\V_{b}\\\vdots\\V_{l}\end{pmatrix}$$

### Equazioni di Tableau
>[!note]
>$$A=\begin{cases}
A\overrightarrow{i}=\overrightarrow{0}& n-1&\text{KCL linearmente indipendenti} \\
A^{T}\overrightarrow{u}-\overrightarrow{v}=\overrightarrow{0}&l&\text{KVL-I linearmente indipendenti}
\end{cases}$$
>
>In questo caso abbiamo $2l+n-1$ incognite, quindi $l+n-1$ equazioni topologiche e $l$ equazioni costitutive. In totale abbiamo quindi $2l+n-1$ equazioni linearmente indipendenti.
