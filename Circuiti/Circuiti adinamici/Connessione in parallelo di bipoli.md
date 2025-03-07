>[!note]
>Due bipoli connessi in parallelo quando sono collegati alla stessa coppia di nodi. I questo caso ogni bipolo ha la stessa caduta di tensione ai loro capi.
>
>Nel caso in cui entrambi i bipoli ammettano base tensione la connessione è sempre possibile: $$\begin{cases}
>i_{1}=f(v) \\
>i_{2}=g(v)
>\end{cases}\Longrightarrow i=i_{1}+i_{2}=f(v)+g(v)=h(v)$$
>Nel caso in cui uno dei due bipoli non ammetta base tensione, la connessione è possibile, e il bipolo risultante è equivalente a quello non definito su base tensione.
>
>Nel caso in cui nessuno dei due bipoli ammetta base tensione, la connessione in parallelo non è sempre possibile, e va valutata caso per caso.

### Partitore di corrente
>[!note]
>![[Pasted image 20250306225203.png|center]]
>Il partitore di corrente è una regola applicata ai resistori lineari connessi in serie. Si ha che, dati i valori di conduttanza $G_{j}$ e la tensione ai capi $i$: $$i_{k}= \frac{G_{j}}{\sum\limits_{k=1}^{M}G_{k}}i$$
>Nel caso $M=2$: $$i_{1}= \frac{G_{1}}{G_{1}+G_{2}}i= \frac{R_{2}}{R_{1}+R_{2}}i\qquad i_{2}= \frac{G_{2}}{G_{1}+G_{2}}i= \frac{R_{1}}{R_{1}+R_{2}}i$$

