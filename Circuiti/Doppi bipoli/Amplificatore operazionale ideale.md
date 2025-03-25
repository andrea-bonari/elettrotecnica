>[!note]
>Un amplificatore operazionale ideale (OP. AMP.) è un doppio bipolo usato per amplificare (o saturare) una tensione. Possiamo definire il suo modello come: 
>![[Pasted image 20250324184703.png]]
>Ha equazioni costitutive:
>![[Pasted image 20240901104633.png]]
>Con $\alpha\in[10^{5},10^{6}]$ guadagno dell'amplificatore.
>Siccome è difficile mantenere l'OP. AMP. in regione lineare di operazione $[-\varepsilon, \varepsilon]$ in anello aperto, introduciamo il concetto di retroazione, cioè l'introduzione di un collegamento in maniera opportuna tra ingresso e uscita, per far si che $V_{o}$ non dipenda da $V_{d}$.

>[!tip] Nullatore e Noratore
>| Simbolo                              | Nome      | Equazione costitutiva                             |
>| ------------------------------------ | --------- | ------------------------------------------------- |
>| ![[Pasted image 20250320123200.png]] | Nullatore | $$\begin{cases}V=0\\i=0\end{cases}$$              |
>| ![[Pasted image 20250320123221.png]] | Noratore  | $$\begin{cases}\forall V \\\forall i\end{cases}$$ |

>[!tip] Definizione di nullore
>Il nullore è un doppio bipolo che ha su una porta un nullatore e sull'altra un noratore.
>![[Pasted image 20250320123345.png]]
>Ha come equazioni costitutive quelle nel nullatore: $$\begin{cases}
>V_{1}=0\\
>i_{1}=0
>\end{cases}$$
>Non ammette basi di definizione canoniche, ma è possibile darne rappresentazione tramite matrice di trasmissione: $$\begin{pmatrix}V_{1}\\i_{1}\end{pmatrix}=\begin{pmatrix}0&0\\0&0\end{pmatrix}\begin{pmatrix}V_{2}\\-i_{2}\end{pmatrix}$$
>Riguardo la potenza: $$p_{a}(t)=v_{2}i_{2}\lesseqgtr0$$
>Sotto opportune ipotesi, il nullore è un modello accurato dell'amplificatore operazionale:
>- L'OP. AMP. sta operando in condizioni di massa virtuale $(V_{1}=0)$
>- La resistenza di ingresso dell'OP. AMP. è infinita ($i_{1}=0$)

