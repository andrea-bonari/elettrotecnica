### Connessione in serie di bipoli
>[!note]
>Due bipoli sono connessi in serie quando sono gli unici due bipoli che incidono su un dato nodo.
>![[Pasted image 20240824160938.png]]
>Di conseguenza i bipoli sono attraversati dalla stessa corrente.

Criteri per la connessione in serie:
##### Entrambi i bipoli ammettono base corrente
La connessione in serie è sempre possibile.
$$\begin{cases}
V_{1}=f(i) \\
V_{2}=g(i)
\end{cases}\Longrightarrow V_{eq}=V_{1}+V_{2}=f(i)+g(i)=h(i)$$
>[!example]
>Nel caso dei resistori: $$V_{eq}=V_{1}+V_{2}= R_{1}i+R_{2}i=(R_{1}+R_{2})i$$
>Nel caso di $n$ resistori: $$V_{eq}=\left(\sum\limits_{k=1}^{n} R_{k}\right)i$$

##### Uno dei due bipoli non è definito in base corrente
La connessione in serie è sempre possibile e il bipolo equivalente è dato dal bipolo non definito su base corrente.
![[Pasted image 20240824162154.png]]

##### Nessuno dei due bipoli è definito su base corrente
Dobbiamo valutare caso per caso se la connessione è possibile.

---

>[!tip] Partitore di tensione
>![[Pasted image 20240824162900.png]]
>
>$$\begin{align*}
V_{k} &=R_{k}i\\
V&= \sum\limits_{k=1}^{N}V_{k}=i\sum\limits_{k=1}^{N}R_{k}\\
\Longrightarrow I&= \frac{V}{\sum\limits_{k=1}^{N}R_{k}}\\
\Longrightarrow V_{k}&= \frac{R_{k}}{\sum\limits_{k=1}^{N}R_{k}}V
\end{align*}$$

### Connessione in parallelo di bipoli
>[!note]
>Due bipoli sono connessi in parallelo quando sono collegati alla stessa coppia di nodi.
>![[Pasted image 20240824163441.png]]
>I bipoli hanno la stessa caduta di tensione ai loro capi.

Criteri per la connessione in parallelo:
##### Entrambi i bipoli ammettono base tensione
La connessione in parallelo è sempre possibile.
$$\begin{cases}
i_{1}=f(v) \\
i_{2}=g(v)
\end{cases}\Longrightarrow i_{eq}=i_{1}+i_{2}=f(v)+g(v)=h(v)$$
>[!example]
>Nel caso del resistore: $$R_{eq}= \frac{1}{\frac{1}{R_{1}}+ \frac{1}{R_{2}}}= \frac{R_{1}R_{2}}{R_{1}+R_{2}}$$
##### Uno dei due bipoli non è definito in base tensione
La connessione è possibile, e il bipolo risultante è equivalente a quello non definito su base tensione.
![[Pasted image 20240824164352.png]]

##### Nessuno dei due bipoli è definito su base tensione
Dobbiamo valutare caso per caso se la connessione è possibile.

---

>[!tip] Partitore di corrente
>![[Pasted image 20240824164627.png]]
>$$\begin{align*}
i_{k}&= G_{k}V\\
i&= \sum\limits_{k=1}^{N} i_{k}=V\sum\limits_{k=1}^{N}G_{k}\\
\Longrightarrow v&= \frac{i}{\sum\limits_{k=1}^{N}G_{k}}\\
\Longrightarrow i_{k}&= \frac{G_{k}}{\sum\limits_{k=1}^{N}G_{k}}i
\end{align*}$$
>Nel caso di due resistori: $$i_{1}= \frac{R_{2}}{R_{1}+R_{2}}i$$

