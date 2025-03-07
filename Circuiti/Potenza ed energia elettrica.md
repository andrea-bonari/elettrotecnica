>[!note]
>La potenza istantanea di un bipolo è definita come: $$p(t)= \frac{\text{d}}{\text{d}t} W(t)= V(t)\cdot i(t)\qquad [p]=\text{W}$$
>Definiamo inoltre potenza assorbita ed erogata. In convenzione normale: $$\begin{align*}
>p_{a}(t)&= V(t)\cdot i(t)\\
>p_{e}(t)&= -V(t)\cdot i(t)
>\end{align*}$$
>

>[!example] Dimostrazione
>Consideriamo un generico bipolo tra i nodi $A$ e $B$, immerso in un campo elettrico. Inoltre consideriamo la tensione $V_{AB}$ e la quantità di carica $\Delta Q$ in $A$.
>Sappiamo che: $$L_{AB}=  \Delta Q\int_{AB} \overrightarrow{E}\text{ d}\overrightarrow{l}=\Delta Q \left(-\int_{BA}\overrightarrow{E}\text{ d}\overrightarrow{l}\right)=\Delta Q\cdot V_{AB}$$
>Siccome il lavoro è una differenza di energia: $$L_{AB}=W(A)-W(B)=\Delta W$$
>E quindi: $$\frac{\Delta W}{\Delta t}= \frac{\Delta Q}{\Delta t}\cdot V_{AB}$$
>E per $\Delta t\to0$: $$\frac{\text{d}}{\text{d}t} W= i\cdot V_{AB}$$

### Potenza istantanea di un n-poli
>[!note]
>Avendo un generico $n$-poli con nodo di riferimento, in convenzione normale: $$p_{a}(t)=\sum\limits_{k=1}^{n-1}v_{k}(t)i_{k}(t)$$

### Teorema di Tellegen
>[!note]
>Avendo un circuito il cui grafo è connesso e contiene $n$ nodi e $l$ lati, orientato in convenzione normale per tutti i lati del grafo, definisco tensioni a correnti compatibili col grafo i seguenti vettori: $$\begin{align*}
>\overrightarrow{i}&= (i_{1},\cdots,i_{n})^{T}\\
>\overrightarrow{v}&= (v_{1},\cdots,v_{n})^{T}
>\end{align*}$$
>Il teorema di Tellegen afferma che $$\overrightarrow{v}\space^{T}\cdot\overrightarrow{i}= \overrightarrow{i}^{T}\cdot\overrightarrow{v}=\sum\limits_{k=1}^{n}v_{k}i_{k}=0$$

>[!example] Dimostrazione
>Usando le equazioni di Tableau: $$\begin{cases}
>A\overrightarrow{i}=\overrightarrow{0} \\
>A^{T}\cdot\overrightarrow{u}-\overrightarrow{v}=\overrightarrow{0}
>\end{cases}$$
>Allora: $$\overrightarrow{v}\space^{T}\cdot \overrightarrow{i}=(A^{T}\cdot\overrightarrow{u})^{T}\cdot \overrightarrow{i}=\overrightarrow{u}\space^{T}A \overrightarrow{i}=0$$

