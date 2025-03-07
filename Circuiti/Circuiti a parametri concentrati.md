>[!note]
>In circuito a parametri concentrati, anche detto LUMP Circuit Model, si assume che la propagazione dei segnali è istantanea. È un approssimazione valida se: $$L_{C}<<\lambda$$
>Dove $L_{C}$ è la lunghezza caratteristica del circuito, e $\lambda= \frac{c}{f}$ è la lunghezza d'onda dei segnali presenti nel circuito.

### Componenti
>[!note]
>Un componente è un modello di un sistema fisico. A ogni componente sono associate delle equazione costitutive che legano variabili descrittive come tensioni e correnti. Di seguito la rappresentazione di un componente:
>![[Pasted image 20250224165223.png | center]]
>><span style="color: lightgreen;">■</span> superficie limite
>><span style="color: yellow;">■</span> morsetto
>><span style="color: aqua;">■</span> terminale
>><span style="color: purple;">■</span> polo (morsetto + terminale)
>
>In base al numero di poli il componente si classifica come $n$-polo.

Utilizziamo tensioni e correnti come variabili descrittive. Per descrivere in maniera esaustiva un $n$-polo sono sufficienti $2\cdot(n-1)$ variabili descrittive ($n-1$ correnti e $n-1$ tensioni), e un legame tra loro, quindi $2\cdot(n-1)$ equazioni costitutive.

### Leggi di Kirchhoff
>[!abstract] KVL-1
>Dato un circuito che opera in regime stazionario, con $n$ nodi e il cui grafo sia connesso, prendiamo uno dei suoi nodi come riferimento $u_{0}$ per misurare il potenziale elettrico e indichiamo con $u_{1},\cdots, u_{n-1}$ i rimanenti potenziali di nodo. Ad ogni istante di tempo $t$, la tensione $V_{kj}$ tra il nodo $k$ e il nodo $j$ è pari a $u_{k}-u_{j}$. 

>[!abstract] KVL-2
>Dato un circuito che opera in regime stazionario, con $n$ nodi e il cui grafo sia connesso, preso un percorso chiuso che passi per $m$ nodi del grafo (ad ogni istante di tempo $t$), la somma algebrica delle tensioni fra i nodi consecutivi che si incontrano lungo il percorso è nulla.

>[!abstract] KCL
>Prendiamo una superficie chiusa orientata che tagli solo terminale e che non attraversi superfici limite dei componenti. Per un circuito che opera in regime stazionario, in ogni istante di tempo $t$, la somma algebrica di tutte le correnti uscenti e entranti dalla superficie orientata sopra definita è nulla.

### Risoluzione di un circuito
>[!note]
>Risolvere un circuito vuol dire ricavare $2l$ incognite, dove $l$ corrisponde al numero di lati. Per farlo devo scrivere un sistema di $2l$ equazioni lineari composto da $l$ equazioni costitutive e $l$ equazioni topologiche (*KVL* e *KCL*) ($n$ è il numero di nodi): $$\begin{cases}
l&\text{equazioni costitutive} \\
n-1&\text{KCL} \\
l&\text{KVL - I}
\end{cases}\qquad\text{linearmente indipendenti}$$

>[!tip] Matrice di incidenza
>La matrice di incidenza $A_{a}$ $n\times l$ è un modo di rappresentare in modo compatto un grafo orientato come correnti di $n$ nodi e $l$ righe. È definita come: $$a_{ij}=\begin{cases}
+1&\text{lato uscente da }i\text{ e entrante in }j \\
-1&\text{lato uscente da }j\text{ e entrante in }i \\
0&\text{non c'è lato che connette }i\text{ e }j
\end{cases}$$
>Le $n$ righe delle matrice sono linearmente dipendenti.
>Una proprietà utile per vedere se la matrice è corretta è:
>$$\sum\limits_{k=1}^{n}a_{kj}=0\qquad\forall j$$
>
>È possibile ottenere una matrice di incidenza ridotta $A$ le cui righe sono linearmente indipendenti rimuovendo una riga qualsiasi di $A_{a}$.

Sia $\overrightarrow{i}=(i_{a},\cdots, i_{l})^{T}$ il vettore corrente delle correnti di lato. Imponendo: $$A\overrightarrow{i}=\overrightarrow{0}$$
Si ottengono le $n-1$ KCL linearmente indipendenti riguardanti i tagli nodali.

Sia inoltre $\overrightarrow{v}=(v_{12},\cdots v_{n-2,n-1})^{T}$ il vettore delle tensione di lato e $\overrightarrow{u}=(u_{1},\cdots,u_{n-1})^{T}$ il vettore dei potenziali di nodo. Imponendo: $$A^{T}\cdot\overrightarrow{u}=\overrightarrow{v}$$
Si ottengono le $l$ KVL-1 linearmente indipendenti.

>[!tip] Equazioni di Tableau
>Queste, insieme sono le equazioni di Tableau: $$\begin{cases}
>A\overrightarrow{i}=\overrightarrow{0}&n-1&\text{KCL} \\
>A^{T}\cdot\overrightarrow{u}-\overrightarrow{v}=\overrightarrow{0}&l &\text{KVL - 1}
>\end{cases}$$
>Queste, sommate alle $l$ equazioni costitutive ci permettono di risolvere le $2l+n-1$ equazioni, che ci permetteranno di identificare univocamente il circuito.
