### Teorema di Thévenin
>[!note]
>Consideriamo bipoli compositi contenenti componenti lineari, adinamici, e tempo varianti, oltre a sorgenti impressive di tensione e corrente. Se il circuito composto dal bipolo composito e dal generatore indipendente di corrente ai morsetti $A-B$ ammette una ed una sola soluzione per qualunque valore di $i$ (il bipolo composito è controllabile in corrente), allora esiste il circuito equivalente di Thevenin.
>![[Pasted image 20250313112048.png|center]]

### Teorema di Norton
>[!note]
>Consideriamo bipoli compositi contenenti componenti lineari, adinamici, e tempo varianti, oltre a sorgenti impressive di tensione e corrente. Se il circuito composto dal bipolo composito e dal generatore indipendente di corrente ai morsetti $A-B$ ammette una ed una sola soluzione per qualunque valore di $V$ (il bipolo composito è controllabile in tensione), allora esiste il circuito equivalente di Norton.
>![[Pasted image 20250313112420.png|center]]

>[!example] Dimostrazione
>Applicando il PSE al circuito: $$i=gv+\underbrace{\sum\limits_{k=1}^{N}g_{K}E_{k}+\sum\limits_{j=1}^{M}\beta_{j}A_{j}}_{N+M\text{ generatori indipendendi all'interno del bip. comp.}}$$
>Passivando i generatori indipendenti interni si ottiene: $$\begin{align*}
>&i\bigg|_{\begin{matrix}E_{k}=0\\A_{j}=0\end{matrix}}=g_{0}v\\
>\Longrightarrow\space& \frac{i}{v}\bigg|_{\begin{matrix}E_{k}=0\\A_{j}=0\end{matrix}}=g_{0}= G_{\text{nr}}
>\end{align*}$$
>Passivando il generatore indipendente $v$ si ottiene: $$i\bigg|_{v=0}=\sum\limits_{k=1}^{N}g_{K}E_{k}+\sum\limits_{j=1}^{M}\beta_{j}A_{j}=A_{\text{nr}}$$
>$A_{\text{nr}}$ è detta corrente di cortocircuito.
>La dimostrazione del teorema di Thévenin è analoga.

### Metodo delle prove semplici
>[!note]
>Nel caso dell'equivalente di Thévenin, supponendo di collegare ai morsetti un generatore di corrente indipendente $i$, è possibile applicare il PSE per ricavare i termini $R_{\text{th}}$ e $E_{\text{th}}$: $$\begin{align*}
>R_{\text{th}}&= \frac{V}{i}\bigg|_{E_{\text{th}}=0}\\
>E_{\text{th}}&= V\bigg|_{i=0}
>\end{align*}$$
>Analogamente, nel caso dell'equivalente di Norton, supponendo di collegare ai morsetti un generatore di tensione indipendente $V$, è possibile applicare il PSE per ricavare i termini $G_{\text{nr}}$ e $A_{\text{nr}}$: $$\begin{align*}
>G_{\text{nr}}&= \frac{i}{V}\bigg|_{A_{\text{nr}=0}}\\
>A_{\text{nr}}&= i\bigg|_{V=0}
>\end{align*}$$

