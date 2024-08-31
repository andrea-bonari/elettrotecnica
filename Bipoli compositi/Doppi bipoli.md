>[!note]
>Definisco uno doppio bipolo come una generalizzazione di un bipolo composito in cui siano presenti $n$ coppie di terminali:
>![[Pasted image 20240830155619.png]]
>Questo oggetto è detto un $n$-porte se $i'_{k}=i_{k}$

>[!tip] Porta
>Una porta è una coppia di terminali a cui associo una coppia $(v,i)$.

Consideriamo il caso specifico di un $n$-porte con $n=2$:
![[Pasted image 20240830155839.png]]

>[!tip] Differenze tra un $4$-terminali e un doppio bipolo.
>- Il grafo di un doppio bipolo ha solo $2$ lati, mentre un $4$-terminali ne ha $3$.

### Doppi bipoli propri
>[!note]
>Un doppio bipolo si dice proprio se le condizioni $i_{1}=i'_{1}$ e $i_{2}=i'_{2}$ è verificata per come è fatto internamente il doppio bipolo.
>![[Pasted image 20240830160430.png]]
>Viceversa, un doppio bipolo si dice improprio se è un $4$-terminali che si comporta da doppio bipolo a seconda del circuito in cui è collegato.
>![[Pasted image 20240830160759.png]]

### Rappresentazione tripolare
>[!note]
>Un doppio bipolo proprio è rappresentabile in modo tripolare se cortocircuitiamo i nodi $B$ e $D$ del doppio bipolo:
>![[Pasted image 20240831101416.png]]
>Questa rappresentazione è identica a quella data per tripoli, è quindi possibile rappresentare tripoli come doppi bipoli:
>![[Pasted image 20240831101750.png]]

### Potenza assorbita
>[!note]
>Rappresentiamo un doppio bipolo a stella con nodo di riferimento $D$:
>![[Pasted image 20240831102421.png]]
>$$P_{a}^{4T}=V_{a}i_{a}+V_{B}i_{B}+V_{C}i_{C}$$
>Possiamo dire che:
>$$\begin{cases}
i_{A}=i_{1} \\
i_{B}=-i_{1} \\
i_{C}=i_{2} \\
V_{B}=V_{A}-V_{1} \\
V_{C}=V_{2}
\end{cases}$$
>E quindi: $$\begin{align*}
p_{a}^{DB}&= V_{A}i_{1}+(V_{A}-V_{1})(-i_{1})+V_{2}i_{2}\\
&= V_{1}i_{1}+V_{2}i_{2}
\end{align*}$$

### Rappresentazioni di doppi bipoli
>[!note]
>Consideriamo doppi bipoli lineari affini, cioè doppi bipoli descritti da equazioni del tipo (rappresentazione analoga a teorema di esistenza e unicità della soluzione): $$A\overrightarrow{v}+B\overrightarrow{i}+\overrightarrow{c}=0$$
>Per il momento consideriamo solo doppi bipoli lineari, cioè con $\overrightarrow{c}=0$. Riscrivo le equazioni costitutive nel seguente modo:
>$$\overrightarrow{u}=M\overrightarrow{w}$$
>Dove $\overrightarrow{u}$ è il vettore delle variabili dipendenti, mentre $\overrightarrow{w}$ è il vettore delle variabili indipendenti. Quindi $\overrightarrow{w}$ è una base di definizione del doppio bipolo.
>Definiamo le basi di definizione canoniche come: $$\overrightarrow{w}=\begin{pmatrix}i_{1}\\i_{2}\end{pmatrix}\qquad\begin{pmatrix}v_{1}\\v_{2}\end{pmatrix}\qquad\begin{pmatrix}v_{1}\\i_{2}\end{pmatrix}\qquad\begin{pmatrix}i_{1}\\v_{2}\end{pmatrix}$$
>Esistono tante matrici $M$ quante le basi di definizione $\overrightarrow{w}+2$:
>- Matrice di resistenza (base corrente)
>$$\begin{cases}
v_{1}=r_{11}i_{1}+r_{12}i_{2} \\
v_{2}=r_{21}i_{1}+r_{22}i_{2} 
\end{cases}\qquad \overrightarrow{v}=\begin{pmatrix}R\end{pmatrix}\overrightarrow{i}$$
>- Matrice di impedenza (base tensione)
>$$\begin{cases}
i_{1}=g_{11}v_{1}+g_{12}v_{2} \\
i_{2}=g_{21}v_{1}+g_{22}v_{2}
\end{cases}$$
>- Matrice ibrida di tipo 1 (base $(i_{1},v_{2})$)
>$$\begin{cases}
v_{1}=h_{11}i_{1}+ h_{12}v_{2} \\
i_{2}=h_{21}i_{1}+h_{22}v_{2}
\end{cases}$$
>- Matrice ibrida di tipo 2 (base $(v_{1},i_{2})$)
>$$\begin{cases}
i_{1}=h_{11}v_{1}+ h_{12}i_{2} \\
v_{2}=h_{21}v_{1}+ h_{22}i_{2}
\end{cases}$$
>- Matrice di trasmissione diretta (base $(v_{2},-i_{2})$)
>$$\begin{cases}
v_{1}=t_{11}v_{2}+ t_{12}(-i_{2}) \\
i_{1}=t_{21}v_{2}+t_{22}(-i_{2})
\end{cases}$$
>- Matrice di trasmissione inversa (base $(v_{1}, i_{1})$)
>$$\begin{cases}
v_{2}=t_{11}'v_{1}+t_{12}'i_{1} \\
i_{2}=t_{21}'v_{1}+t_{22}'i_{1}
\end{cases}$$

>[!tip] Ricavare la matrice di resistenza
>È possibile ricavare la matrice di resistenza $M$ utilizzando le equazioni costitutive del doppio bipolo, oppure usando il metodo delle prove semplici usando due generatori di corrente attaccati alle coppie di terminali:
>![[Pasted image 20240831104138.png]]
>
>Avremo che quando cortocircuitiamo $i_{1}$:
>$$\begin{cases}V_{1}=R_{12}i_{2} \\
V_{2}=R_{22}i_{2}
\end{cases}\iff\begin{cases}
R_{12}= \frac{V_{1}}{i_{2}} \\
R_{22}= \frac{V_{2}}{2}
\end{cases}$$
>E quando cortocircuitiamo $i_{2}$:
>$$\begin{cases}
V_{1}=R_{11}i_{1} \\
V_{2}=R_{21}i_{2}
\end{cases}\iff\begin{cases}
R_{11}= \frac{V_{1}}{i_{1}} \\
R_{21}= \frac{V_{2}}{i_{2}}
\end{cases}$$

>[!tip] Ricavare la matrice di impedenza
>Il metodo è analogo alla matrice di resistenza.

>[!tip] Ricavare le matrici ibride
>Il metodo è analogo alla matrice di resistenza.

>[!tip] Ricavare la matrice di trasmissione diretta
>$$\frac{1}{t_{11}}= \frac{v_{2}}{v_{1}}\bigg|_{i_{2}=0}\qquad \frac{i}{t_{21}}= \frac{v_{2}}{i_{1}}\bigg|_{i_{2}=0}$$
>$$\frac{1}{t_{21}}= - \frac{i_{2}}{v_{1}}\bigg|_{v_{2}=0}\qquad \frac{1}{t_{22}}= - \frac{i_{2}}{i_{1}}\bigg|_{v_{2}=0}$$

### Simmetria
>[!note]
>Un doppio bipolo è simmetrico se è possibile scambiare tensioni e correnti lasciando invariate le equazioni costitutive. In questo caso è possibile scambiare le porte di un doppio bipolo.

Il doppio bipolo è simmetrico se $r_{11}=r_{22}$ e $r_{21}=r_{12}$ nella matrice di resistenza.
Le condizioni di simmetria sono le seguenti:
![[Pasted image 20240831191718.png]]
