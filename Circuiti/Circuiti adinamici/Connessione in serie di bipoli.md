>[!note]
>Due bipoli sono connessi in serie quando sono gli unici due bipoli che incidono su un dato nodo.
>
>Nel caso in cui entrambi i bipoli ammettano base corrente, la connessione in serie è sempre possibile: $$\begin{cases}
>V_{1}=f(i) \\
>V_{2}=g(i)
>\end{cases}\Longrightarrow V=V_{1}+V_{2}=f(i)+g(i)$$
>Nel caso in cui uno dei due bipoli non è definito in base corrente, la connessione in serie è sempre possibile, e il bipolo equivalente è dato dal bipolo non definito su base corrente.
>
>Nel caso in cui nessuno dei due bipoli è definito in base corrente, la connessione in serie non è sempre possibile, e va valutata caso per caso.

### Partitore di tensione
>[!note]
>![[Pasted image 20250306223657.png|center]]
>Il partitore di tensione è una regola applicata ai resistori lineari connessi in serie. Si ha che, dati i valori di resistenza $R_{j}$ e la tensione ai capi $V$: $$V_{j}= \frac{R_{j}}{\sum\limits_{k=1}^{M}R_{k}}V$$
>Nel caso $M=2$: $$V_{1}= \frac{R_{1}}{R_{1}+R_{2}}V\qquad V_{2}= \frac{R_{2}}{R_{1}+R_{2}}V$$
