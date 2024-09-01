>[!note]
>Sotto opportune ipotesi, il nullore è un modello dell'amplificatore operazionale ideale. Il nullore è l'unione di due bipoli patologici: il nullatore e il noratore.
>![[Pasted image 20240901103858.png]]
>Le ipotesi sono:
>- L'amplificatore operazionale opera in condizione di massa virtuale $(v_{1}=0)$
>- La resistenza d'ingresso è infinita ($i_{1}=0$)
>
>Consideriamo un modello più accurato del funzionamento di un OP AMP.
>![[Pasted image 20240901104314.png]]
>Dove $\alpha$ è detto guadagno dell'OP AMP. Solitamente è un valore molto elevato ($\alpha\in[10^{5},10^{6}]$):
>![[Pasted image 20240901104633.png]]
>Per porre $v_{d}$ nell'intervallo $[-\varepsilon, \varepsilon]$, cioè nella regione in cui l'OP AMP opera in modo lineare, tuttavia in anello aperto è molto difficile. Per questo introduciamo il concetto di retroazione:
>![[Pasted image 20240901105014.png]]
>Risolvendo il circuito avremo che $$\lim_{\alpha\to+\infty}v_{d}=0\qquad \lim_{\alpha\to +\infty}v_{0}= - \frac{R_{2}}{R1}E$$

>[!tip] Bipoli patologici
>Un bipolo patologico è un bipolo descritto da due equazioni costitutive.

>[!tip] Nullatore
>![[Pasted image 20240901103154.png]]
>È un bipolo inerte con equazioni costitutive: $$\begin{cases}
v=0 \\
i=0
\end{cases}$$

>[!tip] Noratore
>![[Pasted image 20240901103231.png]]
>È un bipolo attivo con equazioni costitutive: $$\begin{cases}
\forall v \\
\forall i
\end{cases}$$

>[!tip] Nullore
>Il nullore è un doppio bipolo proprio che ha su una porta il nullatore e sull'altra il noratore:
>![[Pasted image 20240901103458.png]]
>Le sue equazioni costitutive sono quelle del nullatore: $$\begin{cases}
v_{1}=0 \\
i_{1}=0
\end{cases}$$
>Il nullore non ammette basi di definizione, possiamo però rappresentarlo tramite matrice di trasmissione diretta: $$T=\begin{pmatrix}0&0\\0&0\end{pmatrix}$$
>La sua potenza assorbita è $$p_{a}^{OA}(t)=v_{2}i_{2}$$

