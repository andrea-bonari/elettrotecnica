### Leggi di Kirchhoff
>[!note] KVL-1
>Dato un circuito che opera in regime stazionario, cioè tutte le tensioni e correnti sono costanti nel tempo, con $n$ nodi e il cui grafo sia connesso, prendiamo uno dei suoi nodi come riferimento $u_{0}$ per misurare il potenziale elettrico e indichiamo con $u_{1},\cdots, u_{n-1}$ i rimanenti potenziali di nodo. Ad ogni istante di tempo $t$, la tensione $V_{kj}$ misurata tra il nodo $k$ e il nodo $j$ è pari a $u_{k}-u_{j}$.

>[!note] KVL-2
>Dato un circuito che opera in regime stazionario, con $n$ nodi e il cui grafo sia connesso, preso un percorso chiuso che passi per $m$ nodi del grafo (ad ogni istante di tempo $t$), la somma algebrica delle tensioni fra i nodi consecutivi che si incontrano lungo il percorso è nulla.

>[!example]
>![[Pasted image 20240823105142.png]]
>Definendo $u_{i}$ come potenziali di nodo e $V_{i}$ come tensioni di lato, possiamo scrivere $l$ *KVL-1*:
>$$\begin{cases}
V_{10}=u_{1}-u_{0}=u_{1} \\
V_{20}=u_{2}-u_{0}=u_{2} \\
V_{12}=u_{1}-u_{2} \\
V_{23}=u_{2}-u_{3} \\
V_{30}=u_{3}-u_{0}=u_{3}
\end{cases}$$
>Scrivo le *KVL-2* alla maglia <span style="color: yellow;">↻</span>:
>$$V_{10}-V_{12}-V_{23}-V_{30}=0$$

>[!note] KCL
>Prendiamo una superficie chiusa orientata che tagli solo terminale e che non attraversi superfici limite dei componenti. Per un circuito che opera in regime stazionario, in ogni istante di tempo $t$, la somma algebrica di tutte le correnti uscenti e entranti dalla superficie orientata sopra definita è nulla.

>[!example]
>![[Pasted image 20240823110715.png]]
>Creiamo un grafo orientato come le correnti:
>![[Pasted image 20240823110841.png]]
>Possiamo dire dai tagli fatti che:
><span style="color: blue;">■</span> $i_{12}+i_{10}=0$
><span style="color: red;">■</span> $i_{24}-i_{43}-i_{50}=0$
><span style="color: lightgreen;">■</span> $-i_{12}+i_{24}+i_{20}+i_{30}-i_{43}=0$

### Risoluzione di circuiti
>[!note]
>Risolvere un circuito vuol dire ricavare $2l$ incognite, dove $l$ corrisponde al numero di lati. Per farlo devo scrivere un sistema di $2l$ equazioni lineari composto da $l$ equazioni costitutive e $l$ equazioni topologiche (*KVL* e *KCL*) ($n$ è il numero di nodi): $$\begin{cases}
l&\text{ equazioni costitutive} \\
n-1&KCL \\
l-n+1&KVL-I
\end{cases}\qquad\text{linearmente indipendenti}$$

>[!tip] Matrice di incidenza
>La matrice di incidenza $A_{a}$ $n\times l$ è un modo di rappresentare in modo compatto un grafo orientato di $n$ nodi e $l$ righe. È definita come: $$a_{ij}=\begin{cases}
+1&\text{lato uscente da }i\text{ e entrante in }j \\
-1&\text{lato uscente da }j\text{ e entrante in }i \\
0&\text{non c'è lato che connette }i\text{ e }j
\end{cases}$$
>Le $n$ righe delle matrice sono linearmente dipendenti.
>Una proprietà utile per vedere se la matrice è corretta è:
>$$\sum\limits_{k=1}^{n}a_{kj}=0\qquad\forall j$$
>
>È possibile ottenere una matrice di incidenza ridotta $A$ le cui righe sono linearmente indipendenti rimuovendo una riga qualsiasi di $A_{a}$.

>[!example]
>![[Pasted image 20240823113916.png]]
>$$A_{a}=\begin{pmatrix}1&0&-1&0&1\\-1&1&0&0&0\\0&-1&1&-1&0\\0&0&0&1&-1\end{pmatrix}$$
>Rimuovendo la prima riga:
>$$A=\begin{pmatrix}-1&1&0&0&0\\0&-1&1&-1&0\\0&0&0&1&-1\end{pmatrix}$$

Una volta ricavata la matrice di incidenza ridotta, calcolo le $n-1$ equazioni KCL facendo:
$$A\overrightarrow{i}=\overrightarrow{0}$$
Dove $\overrightarrow{i}$ è il vettore contenente le $l$ correnti di lato. Le equazioni ottenute saranno linearmente indipendenti e saranno riguardo i tagli nodali.
 
>[!example]
>![[Pasted image 20240823114452.png]]
>Definiamo $\overrightarrow{i}$ come: $$\overrightarrow{i}=\begin{pmatrix}i_{a}\\i_{b}\\i_{c}\\i_{d}\\i_{e}\end{pmatrix}$$Quindi risolvendo $A\overrightarrow{i}=\overrightarrow{0}$ otterremo:
>$$A\overrightarrow{i}=\overrightarrow{0}\iff\begin{cases}
-i_{a}+i_{b}=0 \\
-i_{b}+i_{c}-i_{d}=0 \\
i_{d}-i_{e}=0
\end{cases}$$

Calcoliamo adesso le $l$ *KVL-I* facendo: $$A^{T}\space\overrightarrow{u}=\overrightarrow{v}$$dove $\overrightarrow{v}$ è il vettore contenente le tensioni di lato, e $\overrightarrow{u}$ è il vettore contenente i potenziali di nodo. L'equazioni saranno linearmente indipendenti.

>[!example]
>Ridisegnando il grafo orientato rispetto alle tensioni in convenzione normale:
>![[Pasted image 20240823161423.png]]
>
>Scegliamo come nodo di riferimento il corrispondente della riga rimossa in $A_{a}$. E dai potenziali di tensione ottenuti da quel nodo creiamo il vettore $\overrightarrow{u}$. Quindi:
>$$A^{T}\space\overrightarrow{u}=\overrightarrow{v}\iff\begin{cases}
-u_{1}= V_{01} \\
u_{1}-u_{2}=V_{12} \\
u_{2}=V_{20} \\
-u_{2}+u_{3}=V_{32} \\
-u_{3}=V_{03}
\end{cases}$$

>[!tip] Equazioni Tableau
>Sono le equazioni topologiche linearmente indipendenti sufficienti per risolvere un circuito. $$\begin{cases}
A\overrightarrow{i}=\overrightarrow{0}&n-1&\text{KCL} \\
A^{T}\space\overrightarrow{u}-\overrightarrow{v}=\overrightarrow{0}&l&\text{KVL-I}
\end{cases}$$In queste equazioni avremo $2l+n-1$ incognite ($l$ correnti, $l$ tensioni e $n-1$ potenziali di nodo). In totale avremo $l+n-1$ equazioni topologiche, che sommate alle $l$ equazioni costitutive ci permetteranno di trovare le $2l+n-1$ incognite.


